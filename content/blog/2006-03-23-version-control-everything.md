---
author: admin
date: 2006-03-23 12:44:22+00:00
draft: false
title: Version Control Everything
type: post
url: /2006/03/23/version-control-everything/
categories:
- Software Development
tags:
- Arch
- ArX
- Clearcase
- CVS
- mototone
- Perforce
- RCS
- SCCS
- SCM
- Subversion
- Version-Control
---

The world of SCM and Version control has always been a major part of software development but usually comes as a big shock to new developers. SCM approaches range from global Clearcase systems with multiple sysadmins keeping it humming to single developers creating files with names like *_v01, *_v02.

Many years back, I was kicking off my first project as the leader and also my first project on a non-Vax development platform. All previous projects had used proprietary source control systems which had been in place before I arrived. In this case, I had to put everything in place. I ended up selecting SCCS on Solaris and it did the job for a small project. Its biggest drawback (shared with RCS) was that it was a "single file" system and needed large amounts of scripting to do anything useful on trees of files.

As we transitioned to a hybrid system of Solaris back-end with Windows on the desktop, we needed something which was compatible with both and we arrived at CVS. I was the CVS evangalist in Integral Design from 1996-2000. As with any system, it had problems, most of which were related to the use of the working copies on Samba and having permissions problems and the usual Unix-windows integration annoyances. We used that approach as the client-server setup never worked reliably. But it was free and it had some fine GUIs which made the developers lives easier. I was able to manage the system is my spare cycles.

One of the main problems of CVS was (and is) the lack of atomicity on commit. Simple problems could cause a commit to fail and then your repository was in a mess. The other problem was that on occasion, the non-locking model was simply not appropriate and a hybrid approach was needed.

Over the past couple of years, I have been keeping an eye on replacements for CVS. I have carried out tests on Arch, ArX, monotone, Bazaar and [Subversion](http://subversion.tigris.org/). The only one of those which was seamless across platforms was Subversion. It was actually designed as the replacement for CVS and in that I think they have succeeded.

Apart from Subversion (SVN) being used as the basis for our own internal SCM system, for the past year we have run a trial project on a customer site using it as the source control system. Normally this customer uses Clearcase for everything but in this case there were people scattered over the US who needed access to the source but were not licenced for Clearcase. The trial used a W2K3 Server running Apache integrated with PHP, Subversion, [WebSVN ](http://websvn.tigris.org/)and [Trac](http://www.edgewall.com/trac/). We used [TortoiseSVN ](http://tortoisesvn.tigris.org/)and [RapidSVN ](http://rapidsvn.tigris.org/)on the clients and also gave read-only access via WebSVN for those who just needed "latest version download" capability (and RSS junkies).

The project was quite small and at its peak had eight people using the repository. But it has been a huge success and required minimal management overhead. It just worked. We ran a non-locking model but tested locking on several occasions to make sure it worked (which it did).

TortoiseSVN is a fantastic front-end and it allowed us to boot-strap co-op students into the world of SCM in no time at all. The [Subclipse ](http://subclipse.tigris.org/)plug-in means that Eclipse users do not even have to leave the GUI to version their files. The US based end-users of the code loved it because all they needed was a URL from us to grab whatever they needed no matter where they were.

Most of all, we loved it because it made the idea of versioning files and data a seamless  part of the daily routine. The mindset changed from 'Oh do I really have to put this in Clearcase?' to 'Just in case, I'll pop it into SVN' and two right-clicks later the file was under version control and accessible to all globally.

This gets us back to the title of the post 'Version Control Everything'. Storage is cheap, people make mistakes on files and change their mind on edits and delete things they shouldn't. With a simple install of TortoiseSVN, you can be up and running in minutes and every piece of data you generate could be placed under version control. The benefit? At the very least, you now have that data backed up elsewhere. But far more importantly, you can chop/change/revert in a completely natural way and always have the full history of what you did and why you did it. It is not quite a versioned file system but it is not far off.

The mind-set change is not actually that big. It is far less than trying to convince people to store everything in some hierarchical structured Content Management System. I recommend you try it as an experiment for a few weeks. The great thing about SVN is that if it doesn't work for you, you can blow the whole thing away in a few minutes and you still have all your original files, right where you want them.

If you do try it, let me know via the comments are here. Setting the system up using TortoiseSVN locally on your desktop/laptop is trivial but only you have access to those versioned files. Setting it up on a server using Apache is more challenging (particularly on Windows) but using it means that anyone with network access to that machine can get to your files (with access controls that you define). If you need any tips on this, let me know. We've done both W2K3 and Fedora server installs.

The Register has a very good article [comparing Subversion to Peforce](http://www.regdeveloper.co.uk/2006/03/23/subversion_perforce/). Well worth reading.

[tags]SCCS, RCS, CVS, Subversion, mototone, Arch, ArX, Clearcase, Perforce, SCM, Version Control[/tags] 
