---
layout: post
title: "Perl tidbit: array references"
date: 2013-01-31 06:27
comments: true
categories: 
---

It can be useful to know the difference between `\@a` and `[@a]` for an array `@a` with regard to array references. Take a look at the little script below:

<!-- more -->

``` perl
#!/usr/bin/perl
use strict;
use warnings;

my @a = (1,3,5);

my $r1 = \@a;
my $r2 = [@a];

$r1->[0] = 'x';
$r2->[1] = 'y';

$\ = "\n";

print $r1;
print $r2;
print join ',', @a;
```

which prints:

``` perl
ARRAY(0x155ac98)
ARRAY(0x155abf0)  # different from first
x,3,5
```

`\@a` gives you a reference to `@a`, which you can use to directly modify the array. `[@a]` creates a reference to a new array with the same content as `@a`, handy if you'd like a "copy" of `@a` but do not wish to modify it through the reference.
