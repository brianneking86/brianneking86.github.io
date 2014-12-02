---
layout: post
title: "Using AJAX with conditions"
date: 2014-12-01 23:30:16 -0500
comments: true
categories: 
---

So Javascript week was a tough week. To say the least. I felt like I had no idea what I was doing which I guess I expected to be used to but at least the ever so wonderful Ruby gives you error messages that mean something. Seeing the words "undefined is not a function" is one of the most infuriating things ever in life and thats if you only see it once! Seeing it every 5 seconds slowly picked away at my will to live or at least to continue coding. 

For some reason that I don't understand, at some point during the week things started to make a little bit of sense. By the end of the week, I had a vague idea that I maybe kind of had an inkling of what to do. Of course, all of this meant that I was inevitably going to get super determined to figure out something difficult on my own to prove that I wasn't a total moron. In the case of Javascript I found my "something difficult" during the rails task lister lab. I set up the basic setup with lists that have many tasks and then added boards that have many lists. On the board index page each div would be for a board and the line items would be the lists associated with the board. Seems simple. On the board show page each div would be a list that belonged to that board and the line items would be the tasks associated with that list. This presented a problem if I wanted to be able to add a list from either page. On the board index page, a list would get appended as a line item but on the board show page it would get appended as a whole div with the potential for lines items. I had checked out Trello to make sure I wasn't crazy and that it was possible but it was set up in a way that would have dealt with the issue so of course that meant that my best bet on getting an answer was poor Steven Nunez.

-> ![alt text](https://raw.githubusercontent.com/brianneking86/brianneking86.github.io/source/source/images/board_index.png "Board Index Page") ![alt text](https://raw.githubusercontent.com/brianneking86/brianneking86.github.io/source/source/images/board_show.png "Board Show Page")<-