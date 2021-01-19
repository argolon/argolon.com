---
author: admin
date: 2008-01-19 12:17:24+00:00
draft: false
title: Movable Type - Not there yet
type: post
url: /2008/01/19/movable-type-not-there-yet/
categories:
- Technical
- Tools
tags:
- akismet
- movable type
- MT
- MT4
- OpenID
- widgets
- Wordpress
- WP
---

There has been some new buzz about Movable Type since version 4 was released a while back. I had carried out one install of v3 previously to ensure that we supported it ok in [LouderVoice](http://www.loudervoice.com/). It was one of the worst install experiences I've ever had. I'd prefer to build XEmacs from source on Windows. V3 made me realise why Wordpress had left MT eating its dust. The WP boast of a 5 minute install was not an empty one and it "just works" out of the box in most cases.

Then MT4 came along with lots of hullabaloo and promises of easy install etc. I had another nightmarish time with it due to the fact that they had dropped support for Berkeley DB and I needed to switch to MySQL _before_ upgrading to MT4. I of course found this out afterwards. I also had to get my blog webhost (WebFaction) to update a bunch of its Perl DB libs before I could get the interface to MySQL working.

So finally I got it installed and running and read all about the sooper-de-dooper widget system. But how do I enable it? Drag and drop of widgets into a container like Wordpress? No, I had to hand-edit template files to add support because it is not enabled by default! C'mon, if the competition are doing something better than you and kicking your ass in the market, you damn well better out execute them. Why the hell are there not two sets of templates shipped with a tick-box asking you if you want widget support?

I followed the instructions to the letter and ended up with a sidebar utterly devoid of any styling, just the widget contents dumped into it. I'm sure some MT guru will now slap me and say "oh but you need to enable the tuttifrutti feature as explained in a wiki entry from 2003".

I now have a nightly of MTOS installed so I can test multiple blogs, XMLRPC, ATOM and maybe OpenID. Adding things like OpenID is laudable and will keep the existing user-base happy but if new users can't even try basic basic things like widgets then I'm afraid WP is going to continue to stomp all over MT. Comments about how MT is technically superior to WP are frankly irrelevant to the vast bulk of bloggers.

And where the hell are all the themes for me to try out? A bazillion WP themes and shag-all MT styles if I Google. Add to that an anti-spam system which is a bad joke compared to Akismet and MT just isn't competitive where it matters.

If MTOS is to be something other than a lame-duck piece of code put out to pasture whilst Six Apart focuses on Enterprise and Vox, then they need to get the finger out now. Find 200 Wordpress bloggers willing to give MT a try and do a swathe of monitored user testing with them from downloading the zip to install, to import of posts/comments, to permalinks, to trackbacks, to widgets, to users, to themes, to posting, to spam, to comments. Then fix the product.
