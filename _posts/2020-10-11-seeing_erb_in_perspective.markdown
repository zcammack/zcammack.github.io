---
layout: post
title:      "Seeing ERB In Perspective"
date:       2020-10-12 01:24:55 +0000
permalink:  seeing_erb_in_perspective
---


This week in my studies has been a difficult challenge... Sinatra development has been fairly easy itself, but it brought with it a challenge I was somewhat surprised with. Creating ERB files has proven to be a little more difficult than I had originally imagined... as creating an HTML file proved to be much more time consuming and frustrating than almost anything else possible within the Sinatra program. Still, with practice and a lot of research, I've eventually overcome the hurdle.

Some interesting things I've learned about creating ERB files... it's much more useful to create an ERB file for each specific task I want to accomplish than it is to create one large comprehensive ERB. For example, I originally intended to create a file that would allow me to see an index of objects that every user had created at once. This proved rather awkward with testing... as it meant that my users had no idea what objects they themselves owned. I eventually opted to create a sort of homepage ERB file that would first be displayed for the user. It's whole purpose being that it displayed items specific to the user first with a few buttons to display other information in different ways.

The main takeaway of what I've learned is that ERB files should be specific in their function and that it's important to view things from the perspective of the user first and foremost. While it may make sense to you what your structure should read, it needs to make sense to someone who won't have access to reading what's under the hood.
