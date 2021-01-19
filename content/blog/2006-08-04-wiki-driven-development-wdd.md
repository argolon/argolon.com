---
author: admin
date: 2006-08-04 08:06:22+00:00
draft: false
title: Wiki Driven Development (WDD)
type: post
url: /2006/08/04/wiki-driven-development-wdd/
categories:
- Software Development
tags:
- MediaWiki
- MoinMoin
- PBWiki
- SocialText
- SocialText-Open
- WDD
- Wiki
- Wiki-Driven-Development
---

[Jason Kolb coined this great term](http://jasonkolb.typepad.com/weblog/2006/07/wikidriven_deve.html) a few weeks back and it has stuck in my head. He is writing the end-user documentation in the wiki before he starts development. Our scope is slightly less ambitious and that is simply to use a wiki as the initial requirements management tool for the first time.

In my first job back in 1745, all of our documentation was still being done using variations on troff. I still have the mental scars from that, particularly when we tried to do "diagrams" with it. In some cases, coding the docs was harder than coding the system. Then for years we all used Word and Frame and I hated both. Wordprocessors and DTP packages are about display and presentation, not content. I never felt they worked in sync with my thinking, I was constantly fighting them. Things improved slightly when I switched to using outline mode in Word so I could focus on the content and its structure but it was clunky and lacked a lot of the features of a decent outliner. 

About two years ago I started using a combination of [Freemind ](http://freemind.sourceforge.net/)and [Leo ](http://webpages.charter.net/edreamleo/front.html)and they have been working extremely well for me. Freemind is awesome when you have a ton of information and ideas coming at you in an area you are not expert in. It allows you to cluster related items together in an iterative way until you have a good high-level view of what you are dealing with. I usually stop using it at that point and switch to Leo. 

Leo is a classic outliner tool and is fantastic for structuring all of the content once you have a handle on it. It is a wonderfully extensible tool and is of course written in Python. We spent a week with a customer at the start of this year gathering requirements and I just typed the brain-storms live into Leo each day and re-ordered and made sense of it each night. Once they were happy, I was able to spit a Word doc out, tart it up a bit and we had the full requirements document back to them in a few days. They loved it. 

Of course the OPML editor is another possibility here but I simply hate the UI and do not find it anywhere near as intuitive as Leo.

For our new venture. I thought I would experiment with using a wiki to document the requirements and specs. I chose MediaWiki as the platform and I have been shocked by how well it is working for me. I finally have a tool which allows me to write without getting in the way. I generate new page titles on the fly with no content, I can link internally and externally with a trivial markup syntax and for the first time ever, I don't want a WYSIWYG editor. I spend my entire time concentrated on the content and its relationships and the tool simply fades into the background. The killer feature is that structure turns into view. I can have a hierarchical view of the content but that is just one view. I simply create summary pages of links to content depending on the aspect I am interested in.

All of the extra goodies are just icing on the cake - collaborative writing, instant publishing, RSS feeds for updates, easy portability of the DB from system to system, almost zero learning curve for new people, no doc distribution, single source and everything viewable and editable in a browser on any platform. There is obviously the usual danger with wikis that it becomes a disorganised mess of pages but so far I am not finding that at all and will continue to work within it until it stops making sense. 

One area I need to look at is per-page security. It would be great to just allow outsourcers to have access to certain areas of the Wiki and not to others. Hell, they could even contribute to it and we would have no more of the doc/pdf ping pong I have done for 14 years. At the moment I just have the entire wiki locked down. I think there are some extensions which may enable me to get this fine-grained protection.

As far as platforms are concerned, I've looked at a few. There is a [great comparison page over at WikiMatrix](http://www.wikimatrix.org/) where you can compare any combo of wikis side by side but here are my basic observations: 

[Mediawiki ](http://www.mediawiki.org/wiki/MediaWiki)is the software underpinning Wikipedia and so has a certain pedigree. Things I like are: Trivial install, DB store, support docs, easy markup, easy to use. Things I don't like are: RSS feeds causing problems on some feedreaders, awkward to change layout, very little GUI config.

[SocialText Open](http://sourceforge.net/projects/socialtext/) was just launched last week and is the OpenSource version of their enterprise wiki product. I loved the sound of the feature-set but when I downloaded it and read the install doc, I went no further. Lines like "Some 150+ CPAN modules are required, some of which don't have prebuilt packages for your OS" and "In its current form, Socialtext dominates Apache. We hope to change that in the near future, but for now Socialtext expects to own the entire Apache configuration". I'll have a look again when they have an install that is as easy as MediaWiki.

[MoinMoin ](http://moinmoin.wikiwikiweb.de/)is written in Python and has a good feature set. Things I like are: Look n Feel, easier to customise, slicker user experience overall. Things I don't like are: File-based storage, install a bit awkward, markup not 100% same as MediaWiki and just a general sense that I don't know the impact of certain actions. I'll keep playing with MoinMoin in the background but I'll stick with MediaWiki for the time being.

If you want to try the wiki approach to requirements and sepcifications, you can use one of the hosted ones like [PBWiki](http://pbwiki.com/) and play. You may find that it suits you too.

[tags]Wiki, Wiki Driven Development, WDD, MoinMoin, MediaWiki, SocialText, SocialText Open, PBWiki[/tags] 
