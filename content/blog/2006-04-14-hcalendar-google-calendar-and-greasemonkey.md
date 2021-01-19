---
author: admin
date: 2006-04-14 19:09:23+00:00
draft: false
title: hCalendar, Google Calendar and Greasemonkey
type: post
url: /2006/04/14/hcalendar-google-calendar-and-greasemonkey/
categories:
- microformats
- StructuredBlogging
tags:
- Airset
- Eventful
- Flock
- Google-Calendar
- Greasemonkey
- hCalendar
- IE7
- microformats
- Structured-Blogging
- Upcoming
---

On my [personal blog](http://conoroneill.com/), I discuss [structured blogging](http://www.structuredblogging.org/) and [microformats](http://microformats.org/) quite a bit, but usually in the context of things like food. However, the opportunities being presented by microformats apply in many different spheres. It is surprising how few startups seem to be building compelling applications using them.

To take one example, online calendars are now two a penny. In many cases there is little to choose between them. Most recently, I have found [Airset](http://www.airset.com/) to be the most functional from an integration to Phone/Palm/etc perspective. Most of the others seem to think that we all have always-on internet connections. Some, like [Eventful ](http://eventful.com/)and [Upcoming ](http://upcoming.org/event/67393/)are in the same space but are really concentrating on events rather than personal calendaring. And now [Google Calendar](http://www.google.com/calendar/render) has launched with a bit of both but without any decent syncing capabilities like Airset or good old fashioned [Yahoo Calendar](http://uk.calendar.yahoo.com/).

All of this is going on, yet the excellent [hCalendar microformat](http://microformats.org/wiki/hcalendar) and associated structured blogging plug-in for [Wordpress](http://wordpress.org/) are barely being leveraged at all. Some, like Eventful, do seem to be interested in it but I see no reall buzz or activity. I had thought maybe it was a "hard" problem.

hCalendar is a way of describing calendar information so that things like event announcements can not only be presented on a blog or web-page, but they can be intelligently interpreted and used by software. One feature lacking in all of the online event and calendar applications is the ability to give them my blog address and have them scan the blog automatically for Events I have published and load them into the application for me and others to see in some centralised location with other related events.

Yesterday on the microformats mailing list, [Mark Pilgrim set a challenge](http://microformats.org/discuss/mail/microformats-discuss/2006-April/003669.html): He offered to donate a free copy of 'Greasemonkey Hacks' to the first person to write a Greasemonkey script that adds a "remind me with Google Calendar" button next to any event described in hCalendar.

To explain this a bit further, I'll paraphrase [the explanation of Greasemonkey](http://en.wikipedia.org/wiki/Greasemonkey) from Wikipedia "It is an extension to the Firefox browser that allows users to install scripts that make on-the-fly changes to specific web pages. The changes made to the web pages are executed every time the page is opened, making them effectively permanent for the user running the script.  Greasemonkey can be used for adding new functionality to webpages like embedding price comparison in amazon.com webpages.

So for an end-user who uses Firefox to browse the web, has Greasemonkey installed and has a script which fulfills the challenge set above, blogs which have published Event information appear differently to normal. What happens is that the script would scan each page as it loads. When it sees event info, it inserts a button on the users display of that web-page. When the user clicks the button, the event information is grabbed and passed to Google Calendar and the user can now do one more click and have the event information in their calendar.

I was shocked when Scott Reynen [published a script which does exactly that](http://microformats.org/discuss/mail/microformats-discuss/2006-April/003679.html) the following day! You can grab [Firefox here](http://www.mozilla.com/firefox/), get [Google Calendar here](http://www.google.com/calendar/render), [Greasemonkey here](http://greasemonkey.mozdev.org/) and [the script here](http://randomchaos.com/software/firefox/greasemonkey/googlehcalendar/googlehcalendar.user.js) if you really want to try it out. You can then go to my personal blog at conoroneill.com, scroll down to one of the events I have listed and you will see the relevant button.

Now this is all very geeky and techy. Of course anyone can just manually add those buttons to their event listings on their blog but those buttons are specific to Google. The long-term aim could be for you to tell the system what your calendar application is and the button would automatically send the event information directly to it. Now, imagine if all of the above was embedded in your browser so whenever you were browsing sites which publish events in hCalendar format, two clicks later and that information is in your Calendar. Imagine if Microsoft integrated that into IE7 and Outlook. Imagine if it also grabbed the hCards of the people arranging the event so you now have all their contact details. I assume the Flock browser under development will have these features?

And those are the simple cases. There is so much opportunity here and all it will take is a little push from one of the big guys to start the snowball.

[tags]hCalendar, Structured Blogging, Microformats, Google Calendar, Eventful, Airset, Upcoming, IE7, Flock, Greasemonkey[/tags] 
