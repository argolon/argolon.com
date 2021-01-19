---
author: admin
date: 2005-12-10 00:11:27+00:00
draft: false
title: Open issues on Python development
type: post
url: /2005/12/10/open-issues-on-python-development/
categories:
- Argolon
- Software Development
tags:
- Database-API
- mysql
- ODBC
- oracle
- Python
- SQL-Server
---

As mentioned in a previous post, we have been having great success recently using Python as a develoment language for both customer engagements and our own internal long-term projects. There are however, some areas where we have to make decisions in its usage. 

The first is quite simple - development environment. The options are currently quite limited: The PythonWin IDE, Eclipse with PyDev or "Insert Name of One True Editor Here"+ CLI. At the moment we are mainly using the Eclipse approach but have doubts over things like performance and debug features. Opinions (not flame wars) would be genuinely appreciated particularly in the area of scalability for large applications.

The second is database access. In most of our developments, we strive for cross-platform capability, generally targetting W2K/W2K3, Linux and sometimes Solaris. Ideally for systems where there is no Stored Procedure development on the DB, we aim for DB independence too with SQL Server, Oracle and MySQL being the top three that we have to deal with. 

Unfortunately most developers in recent years are very Windows centric and start using ODBC by default. The big advantage of Java is that the JDBC API works on every platform that Java supports and is available for pretty much every mainstream DB going. In the case of Python, the options are ODBC or the native DB API. The ODBC driver works fine but obviously only on Windows. The [Database API itself](http://www.python.org/peps/pep-0249.html) is solid and in theory gives us DB independence but we have been concerned about the variable quality and level of development on the various DB-specific modules which are required.

We are interested in hearing from other Python developers who do heavy-duty DB related development on a variety of RDBMS what their experience is of the stability and feature-set of the various modules.

[tags]Python, ODBC, Database API, SQL Server, Oracle, MySQL[/tags] 
