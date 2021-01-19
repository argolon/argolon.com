---
author: admin
date: 2005-12-10 00:36:01+00:00
draft: false
title: Enterprise readiness of Jython?
type: post
url: /2005/12/10/enterprise-readiness-of-jython/
categories:
- Argolon
- Software Development
tags:
- Coyote
- Eclipse
- Enterprise
- Enterprise-level
- JyDT
- Jython
- Netbeans
- PyDev
- Python
---

In our first Python post we mentioned that there can be push-back on the usage of Python in solutions for customers, particularly if the entire system is to be built in Python.

An interesting alternative which can gain more customer acceptance is [Jython](http://www.jython.org/). This is Python reimplemented in  Java and it provides features which are compelling both from a technical perspective and customer acceptance perspective. To the customer, Jython can be viewed as simply another part of a Java based solution where it is providing some scripting, automation and high-level glue. For the developer, it opens up the facilites of Java to the Python interpreter and all the facilites of Python to the JVM.

Tim Bray (Mr XML, now in SUN) has  [a particularly good blog posting](http://www.tbray.org/ongoing/When/200x/2004/05/03/Pedroni) on it.

So, in theory, we like it a lot, and we are particularly looking at it for integrating together existing Java sub-sytems from other vendors and from our customers. However, we are concerned about the history of its development which has been very stop-start and also the lag between it and the mainline Python interpreter. The alpha status of the current release would obviously have to change before we could consider doing a major customer development in it.

Are there any developers using this for Enterprise-level software with actual live, stable deployments in the field? If you are wondering what we mean by "Enterprise-level", an example would be the system we delivered to a customer last December which has had 100% uptime over the past 12 months.

Tim Bray [mentions that Propylon have deployed Jython systems in the field](http://www.tbray.org/ongoing/When/200x/2004/12/08/DynamicJava), which is very interesting.

Additionally, as with the previous post, we are interested in feedback on development environments for Jython. We are currently playing with both [PyDev](http://pydev.sourceforge.net/) [JyDT](http://jydt.sourceforge.net/) and  along with Editor+CLI and [Coyote ](http://www.tbray.org/ongoing/When/200x/2004/12/08/DynamicJava)on [Netbeans](http://www.netbeans.org/). 

[tags]Python, Jython, Enterprise, Enterprise-level, Eclipse, PyDev, JyDT, Netbeans, Coyote[/tags] 
