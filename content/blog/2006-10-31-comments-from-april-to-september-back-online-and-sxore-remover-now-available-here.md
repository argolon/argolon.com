---
author: admin
date: 2006-10-31 10:18:09+00:00
draft: false
title: Comments from April to September back online and sxore remover now available
  here
type: post
url: /2006/10/31/comments-from-april-to-september-back-online-and-sxore-remover-now-available-here/
categories:
- Administration
- Software Development
- Suppliers
- Technical
---

As regular readers know, I used the [sxore ](http://www.sxore.com/)comment system on this blog from April to September. Whilst the intent of sxore was good, the reality fell far short. It was a big mistake handing over my comment data to a third party where that data was not transparently available to me if I ever wished to stop using their services.

I finally bit the bullet a few weeks ago and turned off sxore due to the serious bugs and lack of development on the important features of the system. This meant that all comments from the "sxore era" disappeared off this blog. This annoyed me sufficiently that I spent the odd spare minute between business plan iterations fiddling around with some code to get my content back.

Last night I finally cracked it and pulled all of the sxore comment data into Wordpress. I haven't programmed in anger in a very long time and it was frankly embarrassing trying to do even the simplest things. Programming is not like riding a bicycle, it is more like playing the piano - without practice, that part of your brain bit by bit becomes dull. Still, it was a bit of fun which provided some distraction when the numbers in the financial spreadsheets all started swimming before my eyes. Let me know if you spot any major glitches.

The script will:



* Insert comment_content into wordpress
* Insert comment_author into wordpress
* Insert comment_date into wordpress
* Insert author_url into wordpress


Outstanding issues include:

* Seeing some blank comments in sxore which are not imported (not sure if we have data loss there)
* Seeing some comments with no date in sxore which are marked with the date of the previous comment
* No ability to retrieve email addresses of commenters
* No ability to "thread" comments
* comment_date_gmt set to same as comment_date


If you are in the same boat that I was and wish to revert to standard Wordpress comments, then I'm happy to share the code (despite its shocking dreadfulness).  The script is written in Python so you will need to install that to run it. I highly recommend [Activestate Python](http://www.activestate.com/Products/ActivePython/?tn=1), not just because it is a good distro but also because it is very ironic. It also requires the [MySQLdb](http://sourceforge.net/projects/mysql-python) extension and the [Beautiful Soup](http://www.crummy.com/software/BeautifulSoup/) extension.

One of the taglines for our new venture is "your data on your site under your control". If only I had realised the importance of that line back in April, I could have avoided a lot of wasted time and effort.

Technorati Tags: [sxore](http://www.technorati.com/tags/sxore), [sxore_remover](http://www.technorati.com/tags/sxore_remover), [sxore+remove](http://www.technorati.com/tags/sxore+remove), [Python](http://www.technorati.com/tags/Python)

