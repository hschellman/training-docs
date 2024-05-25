---
layout: lesson
root: .  # Is the only page that doesn't follow the pattern /:path/index.html
permalink: index.html  # Is the only page that doesn't follow the pattern /:path/index.html
venue: "Online"
address: "online"
country: "us"
language: "en"
latitude: "45"
longitude: "-1"
humandate: "May 24-25, 2023"
humantime: "8:00 am - 3:00 pm"
startdate: "2023-05-24"
enddate: "2023-05-25"
instructor: ["Heidi Schellman"]
helper: ["mentor1", "mentor2"]
email: ["Heidi.Schellman@oregonstate.edu"]
eventbrite:
---

This tutorial provides resources for the basics of High Energy Physics Computing

1. How to install common software
2. How to use the ROOT data analysis framework
3. Pointers to tutorials on scripting and git code management


<!-- this is an html comment -->

{% comment %} This is a comment in Liquid {% endcomment %}

> ## Prerequisites
>
> Command line experience is necessary for this training. We recommend the
> participants to go through
> [The Unix Shell](https://swcarpentry.github.io/shell-novice/), if new to the
> command line (also known as terminal or shell).  
{: .prereq}

> ## Getting Started
>
> First step: follow the directions in the "[Setup](
> {{ page.root }}/setup.html)" to arrived prepared for this event. Follow the instructions; we give you an easy exercise 
> to make sure you are good to go.
{: .callout}


<h2 id="schedule">Schedule by Day</h2>

The official schedule for this event is listed on the [Indico site (59762)](https://indico.fnal.gov/event/59762/timetable/#20230524).

{% include sc/schedule.html %}

<!--<center><img  alt="" src="fig/Schedule_computing_training_202105.png"/></center>-->

<!-- An [asynchronous session]({{site.baseurl}}/asynchronous/) is designed as later day acivities for the first two days of the workshop.-->

{% include links.md %}
