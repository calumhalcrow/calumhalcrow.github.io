---
layout: page
title: "Projects"
date: 2014-01-26 04:30
---

Here's a run-down of some of the projects I've been involved in. The "Tech stack" underneath each lists major technologies used in the project, in particular the ones I am most familiar with.

### [Mindvalley](http://mindvalley.com)

Up until April 2014 I worked at Mindvalley, developing web-apps that supported their core business. Because Mindvalley market and sell wellness products, their portfolio of internal apps include: sophisticated campaign tracking services, an e-commerce platform, <abbr title="Email Service Provider">ESP</abbr> integrations and more, all of which I helped develop.

Tech stack: [Ruby][33], [Rails][32], [RSpec][29], [Capistrano][35], [PostGreSQL][4], [MongoDB][36], [Linode][37].

[33]: http://ruby-lang.org
[35]: http://www.capistranorb.com
[36]: http://www.mongodb.org
[37]: https://www.linode.com

### [Binary.com](http://binary.com)

I worked on Binary.com, a provider of fixed-odd financial contracts, as an employee of Regent Markets (the site's owner) for six years. The service has a large user base, and I worked to maintain and bring it forward. I learned a lot about the dynamics of a software company during my time there, from how to have the discipline to write high quality code when everyone wants things done yesterday, to the difficulties of managing a team of developers in a fast-paced company with (seemingly) tonnes of priorities. Definitely my pragmatism, attitude toward Getting Things Done, and general maturity as a software developer was carved into me at RMG.

Tech stack: [Perl][1], [Moose][2], [Mojolicious][24], [Catalyst][3], [PostGreSQL][4], [CouchDB][5], [Redis][25], [JavaScript][6], [JQuery][7], [Apache][8], [Nginx][9], [Jenkins][10], [Git][11], [Debian][12].

### [BukitGasingTrails.info](http://bukitgasingtrails.info)

This webpage shows a map of Bukit Gasing, a forest park located between <abbr title="Kuala Lumpur">KL</abbr> and <abbr title="Petaling Jaya">PJ</abbr>. I started going to the park shortly after moving to the surrounding area. After visiting several times I felt I wanted to see a map of the trails, but when I searched the web I couldn't find anything accurate. That plus being asked for directions a few times, and the existence of some groups fighting to stop further real-estate development on the park's fringes, I decided that having some accessible, accurate information about the park's features online would be beneficial to the community. After battling with the Google Maps JS API, Ruby's Jekyll and writing a Ruby module (with an RSpec unit test!) that puts together the map's data into a <abbr title="JavaScript Object Notation">JSON</abbr> file, the site was good to go.

I should add that I originally thought Rails would be a good choice to power the back-end (there are quite a lot of map nodes that need to be stored somewhere). It turned out that Rails wasn't a good choice, and I ended up storing my map data on a "My Maps" Google Map, exporting the map to KML and parsing it into the format I wanted with a Ruby module. The one thing I got out of that endeavour though was experience with Rails! I actually grew very fond of the framework and wouldn't mind using it in some other projects.

Tech stack: [Google Maps JS API][26], [Jekyll][27], [Ruby][28], [RSpec][29], [Rake][30], [KML][31], [Rails][32].

[26]: http://developers.google.com/maps/documentation/javascript/
[27]: http://jekyllrb.com
[28]: http://www.ruby-lang.org
[29]: http://rspec.info
[30]: http://rake.rubyforge.org
[31]: http://developers.google.com/kml/documentation/
[32]: http://rubyonrails.org

### [KudosEnglishLearning.com](http://kudosenglishlearning.com)

This is my wife's business website. She is an English Trainer, based in the Klang Valley area but often working across Peninsular Malaysia. The site from a technical point of view lacks bells and whistles, but I see that as a good thing. Easy to maintain, easy for visitors to find the information they're looking for, or get in touch. There are some subtle yet interesting design elements that can be found if you look for them: Web Fonts, CSS3 gradients and HTML5 mark-up. (Oh, and I designed the site myself; which I mention not so much as a complement to my design skills but more as an explanation as to why it looks as it does :-)

Tech stack: [WordPress][13], [DreamHost][14], [HTML5][15], [CSS3][16].

### [Campr](https://github.com/calumhalcrow/campr)

Campr is a webapp that facilitates networking at events. It allows you to see everyone who is at the event you are attending, along with a little bit of information about each person. Based on this, you can single out people you may want to get to know better. The project was started at [Hack Weekend](http://hack.weekend.my), a delightful hackathon series that takes place every quarter in Kuala Lumpur. Working on Campr was a great learning experience, but we've ceased development on the project.

Tech stack: [Python][17], [Django][18], [Tornado][19], [SocketIO][20], [RabbitMQ][21], [SQLite][22], [Heroku][23].

### [WebCamp KL](https://www.facebook.com/webcampkl)

WebCamp is a monthly meet-up of web professionals based in and around Kuala Lumpur. I am a fairly active member of the community, and have helped in minor ways to organise some of the group's events.

### [CunningsburghHeritage.com](http://cunningsburghheritage.com)

A site that I set up some time ago for the Cunningsburgh History Group, a community-based organisation from the village where I grew up. I handed over content administration to the group themselves, so the site largely runs itself.

Tech stack: [MODX](http://modx.com), DreamHost.

[1]: http://perl.org
[2]: http://moose.perl.org
[3]: http://catalystframework.org
[4]: http://postgresql.org
[5]: http://couchdb.apache.org
[6]: http://en.wikipedia.org/wiki/JavaScript
[7]: http://jquery.com
[8]: http://apache.org
[9]: http://nginx.org
[10]: http://jenkins-ci.org
[11]: http://git-scm.com
[12]: http://debian.org
[13]: http://wordpress.org
[14]: http://dreamhost.com
[15]: http://html5rocks.com
[16]: http://css3.info
[17]: http://python.org
[18]: http://djangoproject.com
[19]: http://tornadoweb.org
[20]: http://socket.io
[21]: http://rabbitmq.com
[22]: http://sqlite.org
[23]: http://heroku.com
[24]: http://mojolicio.us
[25]: http://redis.io
