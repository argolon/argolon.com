---
author: admin
date: 2006-02-07 08:33:52+00:00
draft: false
title: Free VMWare Server - transform your software development efficiency
type: post
url: /2006/02/07/free-vmware-server-transform-your-software-development-efficiency/
categories:
- Argolon
- Software Development
tags:
- Efficiency
- ESX
- GSX
- Software-Test
- VMWare
---

One of our customers is rightly a big VMWare fan. We have a test-bed in one of their labs running ESX Server with four VMs  on one rack-mount. The management and maintenance overhead of this compared to four servers? You do the math(s).

If you test software and you don't use VMWare Workstation, ESX or GSX, you are wasting time and money. Create a base VM, store it somewhere safe, make a copy any time you want to do some testing, test using the copy, finish test, delete copy, start from clean again (or heck, just use the snapshot feature). No more hours wasted installing and reinstalling OSes, DBs and test tools. Not only that, but you can use the same image on any of the products on any platform (Windows, Linux etc etc).

Most recently we built some VMs for this customer for their developer laptops. The VMs consist of W2K3 Server, with SQL Server 2000/2005, Oracle 9i/10G, Raptor, Crystal, Subversion/Clearcase, Eclipse and a bunch of developer utilities. So instead of messing up the laptop configs with Oracle 9i vs 10G or SQL Server 2000 vs 2005, they keep all the dev tools inside the VMs and only boot the VM they need when they need it. Each developer can customize their copy if they wish and revert back to the vanilla one at any point. The rest of the time they have a bog standard travel warrior setup on the Windows 2000 Pro-based laptop itself.

So imagine our excitement when we heard that VMWare Server, a replacement for GSX Server was about to be launched for free.

[Byte & Switch](http://www.byteandswitch.com/document.asp?doc_id=88280&WT.svl=news2_1)

[eWeek](http://www.eweek.com/article2/0,1759,1920441,00.asp?kc=EWRSS03119TX1K0000594)

[Virtualization.info](http://www.virtualization.info/2006/02/more-details-on-vmware-server.html)

GSX is like an advanced version of Workstation optimised for running multiple communicating VMs simultaneously, each of which could be running a different OS or OS version. We have used it for the testing of both the client-side and server-side of an application with each part in a separate VM but running on the same physical machine.

This is incredible news for anyone involved in software development. The savings in time and cap-ex alone make this a compelling product to have in your environment.

[tags]VMWare, GSX, ESX, Software Test, Efficiency[/tags] 
