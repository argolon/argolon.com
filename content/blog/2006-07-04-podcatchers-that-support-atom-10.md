---
author: admin
date: 2006-07-04 22:10:55+00:00
draft: false
title: Podcatchers that support ATOM 1.0?
type: post
url: /2006/07/04/podcatchers-that-support-atom-10/
categories:
- Technical
tags:
- Armangil
- ATOM
- Awasu
- Blogbridge
- iPodder
- iTunes
- Juice
- podcast
- podcatcher
- RSS
---

I recently passed comment that the [Juice podcast receiver](http://juicereceiver.sourceforge.net/) could not see the MP3's embedded in [Tantek's feed](http://tantek.com/log/2006/06.html#d19t1547). I assumed wrongly that there was something wrong with the feed. But he pointed out that Juice must not support ATOM 1.0 yet. From what I can see, development on Juice has stalled which is a pity as it is a fine tool.

Tantek says that iTunes 6.0 does support ATOM 1.0 but that is no good to me as I refuse to install software which is built on the basis of controlling users. However I have had no success finding an alternative. I looked at both [JPodder](http://www.jpodder.com/) and [Doppler](http://www.dopplerradio.net/) but they rejected the feed too. Only [Armangil's podcatcher](http://podcatcher.rubyforge.org/) seems to support it but that is a CLI tool which just sounds like too much hard work.

Does anyone know of a Windows podcatcher which does support ATOM 1.0 along with the usual RSS? Need the standard unsupervised downloads etc as features.

UPDATE 1: I've also looked at standard feedreaders like [Blogbridge](http://www.blogbridge.com) and [Awasu](http://www.awasu.com). Neither of them can even parse Tantek's feed. The feed gives some errors in the feed validator but only trivial ones so the problem looks to be at the reader end. Awasu is a nice looking piece of software and does have auto-download of enclosures which is all I really need.

UPDATE 2: I needed to upgrade Awasu to the latest beta for ATOM 1.0 support. It can now see Tantek's and Tim Bray's feeds perfectly. In fact, it now proves that Bloglines is making a complete mess of displaying Tantek's. Next to see if the enclosures are downloaded ok.

[tags]ATOM, RSS, podcatcher, podcast, Juice, iPodder, iTunes, Armangil, Blogbridge, Awasu[/tags] 
