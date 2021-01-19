---
author: admin
date: 2008-01-27 16:16:09+00:00
draft: false
title: Two weeks on Ubuntu
type: post
url: /2008/01/27/two-weeks-on-ubuntu/
categories:
- Reviews
---

Due to major problems with one of our desktops, I donated my main XP desktop to the COO and I decided to use the Ubuntu file server as my desktop for a week "just to see". I'm no Linux newbie, having started with Slackware in 1996 and gone through every iteration of RedHat and Fedora Core since. A few diversions to Suse and Mandriva were failures.

My Linux usage has mainly been server focused but I've often used the desktops either remotely using XWin on Cygwin or in a VMWare virtual machine. However there have always been enough issues to prevent me using it as a primary desktop. The last attempt I made was in Summer 2006 when I ran a dual-boot laptop with XP and Ubuntu. However an inability to get the microphone working, whilst seemingly trivial, made it unusable for video-conferencing, Skype or VOIP.

We recently got a new low-end server mainly for file-serving and running some test VMs for LouderVoice. It is an el-cheapo Dell Vostro 200 and came with Vista Home. I downloaded the latest Fedora Core but I couldn't even get the install DVD to boot. I've been finding Fedora less and less reliable with each new release but this was crazy, they clearly hadn't tested on one of the most common machines out there!

So on a whim, with all the recent positive buzz around Gutsy Gibbon, I decided to install that instead. A previous attempt to install the Ubuntu Server Edition left me with a server alright, but one with almost nothing installed or enabled. This time I installed the Desktop Edition and installed server features as required.

Most reviews of Linux Distros seem to spend the entire time talking about the install rather than the day to day. This isn't one of those. Install was a breeze. Full stop.

The whole apt-get/Synaptic system for installing apps is very easy to use but was required constantly for days as I found (once again) almost nothing installed by default. Call me lazy and clueless but on Fedora, I always clicked the "install everything" option, just in case. So I added mail, DNS, Samba, development tools etc etc. Then I realised I had almost no multimedia stuff so there was a round of that too.

Within a few days I had a set-up that suited me. In fact, many of the apps I use on XP are cross-platform anyway so it wasn't a big change. Firefox, Pidgin, Filezilla, Azureus, Gizmo, Eclipse, XEmacs, Skype, Picasa, MySQL Query Browser, OpenSSH etc etc.

Immediate issues I ran into? Well something I installed lobbed a copy of libstdc++.so.6 into /usr/local which meant I wasted two days trying to get Skype to run before I finally spotted it and deleted it. The use of Python2.5 by default, whilst laudable, causes me issues with running the LouderVoice code. Some of our backend stuff is really only happy with 2.4. You can install both but WX apps (like WinPDB and SPE) get very confused by that.

I was pleasantly surprised to find that eWallet worked ok via Wine. I need to switch to a proper cross-platform (and Symbian supporting) password manager but I need to write a converter first so I'm stuck with eWallet for the moment.

Graphics programs are a mish-mash. GIMP is great but overkill for quick edits. Most of the others are viewers or library managers. I have never been able to successfully use the image editor in Picasa. The screenshot tool does just that. Ideally I want something like irfanview that views and allows simple obvious tasks like crop, scale, save as other format.

Audio is hit n miss. Rhythmbox is a good player but the last.fm support is flaky as hell. BBC web-site was not happy with whatever realaudio stuff was embedded in Firefox. The biggest problem there tho is that I cannot get the microphone working i.e. the exact same problem as two years ago on a different Dell. So I can't Skype or VOIP. Deeply frustrating and no amount of fiddling is helping. So much for ALSA solving all of the Linux audio issues.

There were two huge problems which were frankly unforgivable. I did a system update as instructed during the first week. It included a kernel update. On reboot, Ubuntu got stuck trying to start. Luckily we have plenty of other machines so I was able to Google it. No-one was 100% sure but one tip was to try adding irqpoll to the boot parameters. Now this did work but come on! This is madness! A distro that is trying to target the average punter and you have to know how to edit grub.conf (after you figure out how to add the param so you can boot at all). I have no idea what that param does. It's clearly a kernel issue and my guess is that is what prevented Fedora from installing too. If you don't support common Dell hardware, go home and stop trying to play with the big boys. Yeah yeah, it's a kernel issue not a distro one. Well don't bloody offer it on updates without testing it.

Last week an almost identical issue occurred. This time X.Org was updated and BOOM, half my GUI apps stopped working. More Googling, more forums, more mea culpas. 24 hours later an update is pushed to fix it. Again, lack of testing, lack of Q&A. Say what you like about MSFT but I think they've had one BSOD-causing update in 7 years. And my apps _always_ work.

The one thing that has always stopped me switching away from MSFT is Office. Not that I love it but I get/send lots of Word Docs and I need 100% round-trip compatibility. I have evangelised OpenOffice many times since SUN released it into the wild but it always always always disappoints. My simplest test is to create an empty Word Doc with Heading1, Heading2, Heading3 (all numbered). Save and open in OO. The tabbing on the headings has always been broken. For what, seven years now? So I tried again and it looks like they may have fixed it. I opened our business plan and by-and-large most of the doc is fine but I utterly failed to change the number formatting on the doc variables, rending it useless. Same old same old. 95% is not good enough. 100% or FAIL.

Anything else? Logictech Fusion Webcam totally refuses to work despite a days effort, bluetooth adapter is detected and devices paired but gives errors if I try to _do_ anything with it. I got a low-end OEM graphics card to replace the built-in graphics. It's a GeForce 7300GT which Googling told me was well supported in Linux. I finally got it setup well using the excellent Envy software (which should be offered by default). I still haven't got the DVI output working tho.

Things I really like?  The Compiz OpenGL Desktop rocks! All those 3D rotations etc are way cool (if totally pointless). The machine is very fast to do most things. VMWare works really well. FF is more stable than on XP and overall, most of the time, things just work.

I spend an enormous amount of time in the browser so the OS is becoming less and less important to me. Heck, when I'm out and about, my N95 phone does most of what I need. If this is your type of usage too and you don't do serious MS Office doc interchange, then Ubuntu might be right for you. But it's not right for your mother yet.

P.S. I may keep this as a rolling review, adding bits n pieces as I think of them.
