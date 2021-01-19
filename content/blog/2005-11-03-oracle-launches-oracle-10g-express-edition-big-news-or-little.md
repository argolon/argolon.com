---
author: admin
date: 2005-11-03 06:30:11+00:00
draft: false
title: Oracle launches Oracle 10G Express Edition - Big news or little?
type: post
url: /2005/11/03/oracle-launches-oracle-10g-express-edition-big-news-or-little/
categories:
- Argolon
- Business
- Software Development
tags:
- dbms
- express
- mysql
- oracle
- sqlserver
- toad
---

[Oracle has just launched 10G Express Edition](http://news.zdnet.com/2100-3513_22-5920796.html), a stripped down version of their mainstream DB. The limits appear to be very similar to MSDE or SQL Server 2005 Express (1 CPU, 4GB DB, 1GB RAM). [This should be big news](http://blogs.siliconvalley.com/gmsv/2005/10/hey_kid_try_som.html). Oracle have absolutely no penetration at the low end where MySQL and (funnily enough) MSDE dominate. But some serious issues mean that maybe it isn't such big news after all. 

All of our earliest engagements were on MSDE and then, as they scaled up, the customers transitioned over to full SQL Server 2000. This is presumably one of the models that Oracle is targetting. 

We have used MySQL quite a bit as a back-end for various web-tools like CRM engines etc but the lack of Stored Procs in particular has meant that we have avoided it for any heavy duty data crunching systems. Last weeks launch of MySQL 5.0 changes the game completely. We are currently doing a thorough evaluation of it to test its suitability in places where previously only SQL Server or Oracle would do. 

Of course there are several alternatives, in both Windows and Linux environments. Whilst PostgeSQL and Firebird are both fine relational DB products, their lack of traction in the market means that it can be a tough sell when suggestion a solution to a customer based around them.

Oracle are right to be worried about MySQL 5.0 and not for technical reasons. Nearly every grad we interview has MySQL skills. It really does have the biggest mindshare for younger developers, many of whom have barely heard of Oracle. The rough n ready nature of MySQL has not been a problem due to it being free. A ton of Open Source projects have grown up around it to fill the gaps.

MSDE gained traction for similar reasons - it had no management tools but a rock solid DB engine (despite the performance throttle) which never let us down and it was free. SQL Server 2005 Express comes with some decent tools which really ups the ante for everyone.

And this is the big flaw in the 10G Express release; Oracle Enterprise Manager is a dog of a piece of software and SQL*Plus Worksheet is just an embarassment. How a company of this size can create such an awesome piece of software such as Oracle and then ham-string it with tools which look like they were built in 1996 with AWT just boggles the mind.

We use a variety of tools to interface to Oracle and the only one worth mentioning is TOAD. We have already seen threads on some of the forums where people are begging Oracle to buy Quest Software and ship TOAD with Express Edition. We have to add our voice to this. Whilst the CLI whizzes can manage to build entire data warehousing systems from a DOS prompt, the rest of us need proper tools to deliver on our commitments.

It may be an interesting few months as we watch what Oracle does next. Worst case for them is that they gain no new customers and lose a bunch of revenue as existing clients use the Express Edition instead of the Standard Edition for all of their smaller developments. Best case for them is that they bootstrap a new generation of PL/SQL heads who need something better than MySQL but refuse to use MS products.

UPDATE 1: It is slightly worse than we thought. It does not ship with Enterprise Manager but instead uses some new pretty trivial web front-end. A step backwards. A quick browse on Sourceforge would find a multitude of MySQl tools which far exceed this in capability. In addition, whilst it does ship with the Net8 libraries so you can use it in conjunction with TOAD to connect to remote DBs, it does not have the Net8 Manager and you have to hand-edit tnsnames etc. So far not very impressive. However, the acid test will be whether it can run some of our meatier code successfully and with good performance.

[tags]oracle,dbms, mysql, sqlserver,toad,express[/tags]
 
 
