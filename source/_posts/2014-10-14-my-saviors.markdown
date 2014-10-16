---
layout: post
title: "My Three Saviors so far"
date: 2014-10-14 15:30:32 -0400
comments: true
categories: "Flatiron&nbsp;School"
---

One of the quotes I have heard/seen most often at Flatiron is "You will never know less than you know right now." Personally, one of the first lessons I learned after starting coding is that asking for help/needing help doesn't mean you're stupid. It means you're learning something challenging. That being said, it can be incredibly frustrating when you're pretty sure you're smart but you just can't seem to get past one stupid line of code in a lab!

While struggling through my first two and a half weeks here at Flatiron I am greatful to have found a few resources that have become my saviors (aside from the TA's and fellow classmates of course!)

-> ** - Rubular.com  - binding.pry  - www.ruby-doc.org ** <-

---

-> ** Rubular.com ** <-

![alt text](https://raw.githubusercontent.com/brianneking86/brianneking86.github.io/source/source/images/rubular.png "Rubular website")

Rubular.com helped me defeat what was one of my first enemies here at Flatiron - **Regex!** Oh how I hated regex when I first started with it. It took multiple sit downs with TA's, watching lab reviews, and sitting down at home with Rubular and the advanced regex lab to finally gain understanding. It was brutal. Especially since I know I am far from really having mastered it.

The site itself is simple to use. You enter your test strings and then try out different combindatons of characters and simples as defined in the quick reference until you have properly matched what you wanted to match without including things that shouldn't match. Sounds super simple right??? HA!

Seen below is my regex for the advanced regex hashtag lab. 

![alt text](https://raw.githubusercontent.com/brianneking86/brianneking86.github.io/source/source/images/rubular_filled.png "Rubular website")

I've seen some intense regex online and it still scares the crap out of me but with Rubular.com, I have hope!!

---
-> **Binding.pry** <-

![alt text]( "binding.pry1")

My start with programming was really with VisualBasic which, outside of a company that is largely based in Excel, is not really good for much. However, it's debugging is fantastic. You can step through your code line by line and see exactly what its doing to pinpoint your problem. When starting with Ruby, I didn't know of anyway to do that (or something similar) and it was yet another frustration in each lab I did. Then one glorious day, I learned of binding.pry and how to use it. 

Basically when you need to look more closely at a method, iteration, etc simply type "binding.pry" as appropriate for example within a block of a .each iteration (as shown above). When you next run your code or rspec it will stop the code at that line in your command line and allow you to poke around.

![alt text]( "binding.pry2")

As in the image above, I was able to type in pigeon to get its value from that iteration. From there I can try out all different lines of code right there to find what isn't working and how to fix it! Its a phenomenal tool for debugging when you are lost about what level of a nested structure you're in or what the return value will be etc etc. Just don't forget to "require 'pry'" at the top of your code!!

---
-> ** www.Ruby-Doc.org ** <-

Last but certainly not least is Ruby-Doc.org which is a treasure trove of information on all things Ruby. Need information on the return value of a method on the string class? Looking to learn how .collect works on an array?? This is the place to go! 

![alt text]( "string")  ![alt text]( "array")

![alt text]( "hash")  ![alt text]( "enumerable")

Shown above are clips from the string, array, hash and enumerable pages that tell you the parent class, its specific methods, included modules, etc. Each method listed has a section showing its specific syntax, which arguments are required or optional, its return value, and some text describing how it works. I've referenced these pages while writing code so many times that I made bookmarks to them for easy access. :)

---

I know over my next 10 weeks at Flatiron I'll find more tools to add to my list of saviors but these three will always be there for me and anyone else struggling through learning Ruby!
