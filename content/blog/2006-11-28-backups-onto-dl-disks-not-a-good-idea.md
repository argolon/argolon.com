---
author: admin
date: 2006-11-28 10:51:14+00:00
draft: false
title: Backups onto DL-Disks not a good idea?
type: post
url: /2006/11/28/backups-onto-dl-disks-not-a-good-idea/
categories:
- Technical
---

I've had backup processes over the years which ranged from copying files between machines to fully automated systems using ATLs. I've never been happy with how we did it in Argolon as it was far too haphazard. 

It finally bit me badly a few weeks back when I did a bare-metal re-build of a server due to intermittent but deadly Gigabit Ethernet data corruption (it looks like all recent linux kernels have huge issues with a variety of GigE NICs). Everything was backed up twice to dual-layer DVD and then the machine re-build went well. When I went to restore I was hit with a stream of CRC errors on the disks. Luckily I managed to use older backups plus the reliable bits of the flakey DVDs to recover 100% of the data but the time wasted was ridiculous. 

We have two identical NEC burners in different machines and they both gave dodgy DL disks. I've upgraded the firmware on one and I'm going to monitor behaviour differences.

This finally prompted me to put in place a proper rigorous backup process with daily incrementals plus weekly fulls on the filesystems, daily full SVN and daily full MySQL. There is automatic daily backup to disk to another machine plus weekly backup to single layer DVD with post-verification. A good chunk of this is done with backup-manager, a lovely linux tool which recently added S3 backup too. Of course, I'd need a functioning broadband connection for that to be of any use. I'll probably drop to incrementals on SVN at some point.

Are DL disks known for bad burns? Or are they highly burner specific so that they are non-portable? If so, then post-verification of disks will have to be done on a different machine than the backup one.
 
Technorati Tags: [Double+Layer+DVD](http://www.technorati.com/tags/Double+Layer+DVD), [Dual+Layer+DVD](http://www.technorati.com/tags/Dual+Layer+DVD), [Backup](http://www.technorati.com/tags/Backup), [backup-manager](http://www.technorati.com/tags/backup-manager)

