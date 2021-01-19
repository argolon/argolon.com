---
author: admin
date: 2009-01-18 09:14:43+00:00
draft: false
title: Using Android phone in Ireland
type: post
url: /2009/01/18/using-android-phone-in-ireland/
categories:
- Technical
tags:
- Android
- google
- HTC
- HTC G1
- Ireland
- mcc
- mnc
- o2
- smartphone
- vodafone
- vodafone live
---

I got an unlocked [HTC G1](http://www.t-mobileg1.com/) from the US recently for a project we are working on. This is the first [Google Android](http://www.android.com/) phone and I'll be doing a full review soon. The first thing you have to do is activate the phone with Google and I immediately ran into problems. It turns out you need to add the Irish mobile network Access Points to the phone so it knows how to connect to the internet.

For the purposed of activation I used an O2 broadband dongle SIM but I also use my normal Vodafone phone SIM since I moved to the 1GB ISP data package they now offer for the same €10 price as the old 512MB Live! WAP package.

You should definitely switch if you are on Live. I just discovered that GPS is so slow to lock on the N95-8GB with Live because the A-GPS port is blocked. It now locks in a minute or so compared to 10 minutes before.

Back to the HTC G1:

Follow the [simple instructions](http://modmygphone.com/forums/showthread.php?t=3201) in this forum post to get to the APN-adding screen.

For O2 Ireland the settings seem to be:



* APN Name: O2 IE Internet
* APN: internet
* MCC: 272
* MNC: 02



For Vodafone Ireland they are:








* APN Name: Vodafone ISP
* APN: hs.vodafone.ie
* Username: vodafone
* Password: vodafone
* MCC: 272
* MNC: 01



SMS works fine but I've had no joy with MMS. This is no big deal since I receive maybe 1 MMS a month and never send any.






