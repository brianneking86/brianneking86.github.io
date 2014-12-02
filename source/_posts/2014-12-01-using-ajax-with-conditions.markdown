---
layout: post
title: "Using AJAX with conditions"
date: 2014-12-01 23:30:16 -0500
comments: true
categories: 
---

So Javascript week was a tough week, to say the least. I felt like I had no idea what I was doing which I guess I expected to be used to by then. At least when learning the ever so wonderful Ruby, it gives you error messages that mean something. Seeing the words "undefined is not a function" is one of the most infuriating things ever in life and thats if you only see it once! Seeing it every 5 seconds slowly picked away at my will to live or at least to continue coding. 

For some reason that I don't understand, at some point during the week things started to make a little bit of sense. By the end of the week, I had a vague idea that I maybe kind of had an inkling of what to do. Of course, all of this meant that I was inevitably going to get super determined to figure out something difficult on my own to prove that I wasn't a total moron. In the case of Javascript I found my "something difficult" during the rails task-lister lab. I created the basic setup with lists that have many tasks and then added boards that have many lists. On the board index page each 'div' would be for a board and the line items in that 'div' would be the lists associated with the board. Seems simple. 

-> ![alt text](https://raw.githubusercontent.com/brianneking86/brianneking86.github.io/source/source/images/board_index.png "Board Index Page") <-

On the board show page each 'div' would be a list that belonged to the board and the line items would be the tasks associated with that list. 

-> ![alt text](https://raw.githubusercontent.com/brianneking86/brianneking86.github.io/source/source/images/board_show.png "Board Show Page") <-

This presented a problem if I wanted to be able to add a list from either page. On the board index page, a list would get appended as a line item but on the board show page it would get appended as a whole div with the potential for line items. I had checked out Trello to make sure I wasn't crazy and that it was possible but it was set up in a way that would have dealt with the issue so of course that meant that my best bet on getting an answer was Steven, poor guy.

Of course I grabbed him on his way out the door to freedom and he kindly (if not somewhat begrudgingly) offered to help out. I poorly explained the situation to him (probably about as well as above) and thankfully he understood and explained that the solution was actually not as difficult as I thought. After persisting the new list to the database, the next stop along the way is the create.js.erb file where I just had to create a condition statement that would check the page for specific css elements. To break that down a little bit more, check the page for either something specific to the board index page that won't be found on the board show page, if it finds that element then render one html.erb template otherwise render a different template. Doesn't sound too hard, right?! 

This time amazingly it wasn't. My initial create.js.erb file looked like this.

-> ![alt text](https://raw.githubusercontent.com/brianneking86/brianneking86.github.io/source/source/images/original.png "Board Index Page") <-

Using the method .length in javascript on a certain css selector will allow you to see if that element is anywhere to be found. All you need to do is check the ".length" of a certain element and then render the correct partial. Once I added my conditional, it looks like this.

-> ![alt text](https://raw.githubusercontent.com/brianneking86/brianneking86.github.io/source/source/images/updated.png "Board Index Page") <-

Adding five lines of code and one additional partial that I called "_board_list.html.erb" I had my answer. The "board_list.html.erb" partial contains one simple 'li' line of html. The original "list.html.erb" contained the html for the 'div' and didn't need to be modified at all. 

Honestly the most important thing I learned in all of this is that just because something seems really difficult doesn't mean it is and mostly figuring out the right question to ask is the hardest part. If I wanted to do it, there's a pretty good chance someone else had the same idea at some point and figured out a way. There is so much more to learn of the wonders of javascript/ajax and while I still lovingly refer to the language as "code vomit on the screen", I'm actually totally motivated to learn more :)

-> ![alt text](https://raw.githubusercontent.com/brianneking86/brianneking86.github.io/source/source/images/200.gif "Board Index Page") <-