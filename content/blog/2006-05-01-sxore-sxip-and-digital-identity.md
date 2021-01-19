---
author: admin
date: 2006-05-01 08:35:05+00:00
draft: false
title: Sxore, Sxip and Digital Identity
type: post
url: /2006/05/01/sxore-sxip-and-digital-identity/
categories:
- DigitalIdentity
- Web20
tags:
- Dick-Hardt
- Digital-Identity
- Digital-Identity-2.0
- Infocard
- Kim-Cameron
- sxip
- sxore
---

We recently set up this site to use [sxore ](http://sxore.com/)as our comment handling system. To quote from the [FAQ](http://sxore.com/copy/faq): 

<blockquote>sxore is an identity and reputation system for blog authors, readers and commenters. By acting as an intermediary between blog posts and comments, sxore provides a framework of identity for participants in the blog dialog.......sxore provides mechanisms for commenting, rating, tagging and following blog conversations. Comments, ratings and tags are displayed on the blog author's site; updates to posts you're following are delivered via an RSS feed to your newsreader. 
</blockquote>


sxore is the first practical implementation of the sxip identity architecture. Again from the FAQ: 

<blockquote>A sxip Homesite is a centralized repository of user data. Rather than dealing with different versions of your identity data at numerous sites across the Internet, and remembering a user name and password for each one, a sxip Homesite account consolidates your authentication credentials and identity information on the sxip Homesite. sxip Membersites (that is, other websites that have implemented the sxip Membersite technology) use the authentication and identity data stored on the sxip Homesite for identity-based transactions (like logging in). </blockquote>



[Digital Identity](http://www.sxip.com/) became a dirty word with the failed Microsoft Passport initiative. Many companies, including Microsoft with its [Infocard ](http://msdn.microsoft.com/winfx/reference/infocard/default.aspx)idea, are having another go at making it a success. Kim Cameron at MS has made great strides in promulgating Infocard and fixing all of the mistakes made with Passport. An interesting coincidence regarding this post is that an [Internet Identity Workshop](http://www.identityblog.com/?p=419) starts today  in Mountainview. 

The simplest benefit of these systems is probably the strongest - you don't have to track a multitude of logins and passwords for all of the sites you access when all you wish to do is identify yourself. Another simple benefit (yet to be implemented in sxip) is that of multiple personas. This is what attracted me to it  - on different sites I log on as different personas "me, the home user" or "me, the business person". Being able to switch between these personas whilst avoiding having some password wallet is a compelling argument for the roll-out of systems like sxip. I currently maintain two [eWallets ](http://www.iliumsoft.com/)and a [KeePass](http://keepass.sourceforge.net/) wallet, all of which are full of simple logon details for web-sites. Getting rid of these for all but the most secure sites would be a big gain. Being able to change my details in one location and having that automatically updated on all the member sites would be fantastic.

[sxip ](http://sxip.com/)is fronted by [Dick Hardt](http://blame.ca/dick/) who founded [Activestate](http://www.activestate.com/). As users of ActiveTcl, ActivePython and ActivePerl, we sit up and listen when Dick has something to say. [His presentations on Digital Identity](http://www.identity20.com/media/OSCON2005/) at OSCON 2005 and [ETech 2006](http://identity20.com/media/ETECH_2006/) are now legendary. I highly recommend you watch them but try not to be distracted by the amazing delivery and focus on the content.

Clearly, sxip has a big battle on its hands with Infocard but if they can start getting some traction initially with some of the big open source sites and then with some of the big Social Media sites, they stand a good chance of success. Also, returning to the topic of some of my recent posts, the mobile internet is one area where first mover advantage may be critical. 

Moving on to sxore, there are good and bad points. As a comment system, it is slick, reliable, good at weeding out spam and the rating system is a nice touch. The single biggest issue is that all of the comment content is stored on their servers not your blog. So if you ever uninstall sxore, you lose all your comments. One of the developers contacted me to ask if full content RSS feeds and a sxore-Wordpress import system would allay my fears. I indicated that it probably would and enabled sxore on this site as a result. 

Some usability issues remain. First, none of the "recent comment" systems work with sxore. Second, it is adding "Post a comment" buttons to Pages which have been identified as "non commentable" in Wordpress. I am not 100% convinced that sxore will get huge traction with bloggers but I am willing to test run it for a few months, if only to help them iron out any bugs. The addition of multiple personas to sxip really is necessary for sxip and sxore to grow.

[tags]sxip, sxore, Digital Identity, Digital Identity 2.0, Dick Hardt, Infocard, Kim Cameron[/tags] 
