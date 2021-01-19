---
author: admin
date: 2005-12-09 23:46:35+00:00
draft: false
title: The power of so-called scripting languages
type: post
url: /2005/12/10/the-power-of-so-called-scripting-languages/
categories:
- Argolon
- Software Development
tags:
- Activestate
- bi
- Business-Intelligence
- Opsware
- Perl
- productivity
- Propylon
- Python
- TCL
- Tk
---

We have always been big fans of development languages which have traditionally been referred to as scripting languages. 

Going back over 10 years, we created some very useful tools and automation systems using [TCL](http://www.tcl.tk/). This may seem like an odd niche choice, but for us, at the time, it had some major advantages. It was cross-platform, it could easily interface to hardware systems like serial ports and it had a great third-party tool called [FreeWrap ](http://freewrap.sourceforge.net/)which allowed one to create executables and not require our end-customers to install the full Tcl package. 

The main drawbacks were the syntax, the fact that no-one had experience in it at the time (strangely, we have seen it on several CVs over the past year!) and the maintainability of large systems developed in it. Another problem was stability from a support perspective - We have never seen a language go through so many backing companies.

In more recent times we, surprisingly, have had some big successes using good old [Perl](http://www.perl.org/). This was a customer driven requirement and worked out very well for us. A major attraction was the number of add-on packages available. However, its reputation as a source of spaghetti code and the difficulty in creating standalone executables  which are easily deployable and installable means that we generally do not pitch it unprompted to customers.

There is one language which we first looked at over five years ago. Even back then it was impressive, now it is genuinely superb. It is, of course, [Python](http://www.python.org/). We are using it in a multitude of ways right now. Everything from simple glue code to automate file transfers across secure links to data transformation tools and DB maintenance. 

The reason we used the phrase "so called scripting languages" is that we are seeing more and more that Python can be far more than the glue, it can be used to build entire systems.  One of the more famous ones was the first version of [Opsware's](http://www.opsware.com/) Datacenter Automation system. We have built several protoypes recently of data-intensive applications and the scalability was exactly where we needed it to be.

It is well known that developer productivity is much higher with languages like Python, but we have been shocked by the multiplier. We have recently been involved in the re-architecture of a system originally built over the space of a year in C++. The guts of it were re-implemented in Python in less than a month with very similar performance.

However, with the notable exception of companies such as [Propylon](http://www.propylon.com/), we have seen very little traction for Python in Irish enterprises. It would be interesting to get some feedback from other development groups working into Ireland on reaction to and acceptance of proposals for systems built entirely on Python foundations. 

When discussing customer requirements we always focus on the business issues first and avoid getting into technical nitty-gritty too early. Of course, many customers want to discuss the solution before they fully uinderstand what they want us to solve. 

The issue with Python is that such customers have probably not heard of it and when it is proposed as a possible implementation route, the customers can go immediately into risk-avoidance mode. They are completely right in having this reaction. But as Python gains more traction, hopefully the recognition of its capability will go up and the objections decrease.

For our own internal developments, we are relying more and more on it. We have some interesting prototypes in progress in the area of Business Intelligence which leverage its many advantages to the full.

An interesting note about the three languages mentioned above is that our distribution of choice in each case has always been from one company - [Activestate](http://www.activestate.com/). These guys really are on the same wavelength as ourselves.

[tags] TCL, Tk, Perl, Python, Activestate, Opsware, Propylon, productivity, Business Intelligence, BI[/tags] 
