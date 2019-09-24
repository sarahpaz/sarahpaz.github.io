---
layout: post
title:      "The Adventures of Adding JavaScript to My Rails App"
date:       2019-09-24 04:32:57 +0000
permalink:  the_adventures_of_adding_javascript_to_my_rails_app
---

The funny thing is, I've actually been introduced to JavaScript before Ruby and we used to be friends. But now, well.. relationships take work, and if there's one major takeaway I got from this project it's that the most is learnt through building. To best understand what's happening, you need to make it and break it, or at least that's what works for me. 

First off, I'll briefly explain the concept behind my Rails app, and then get into the details of adding JavaScript. 

## Boost - Run to Raise - Run Tracking App
My Rails application is pretty simple. It's a run tracking app that allows users to raise money towards a charity of their choice with every run they track. The users also have the ability to add a new charity if one they'd like to contribute to isn't already listed.

(If you want to check it out, the video demo can be found [here](https://youtu.be/7alcGstEa_I).)

## Now the Fun Part... Adding JavaScript (yaaaaaay...) 
I used JavaScript in this application to manipulate the DOM for the charity index and show pages. I set up a clickevent on the Charities link in the navbar by selecting the link class, prevented the default behaviour on click, set up a fetch request to my /charities.json endpoint and accessed the JSON objects to display on the page. Sounds simple right? Some parts were, but others definitely gave me a hard time and I'm still digging my way to understand certain behaviours. But I guess that's part of the beauty of programming, the continuous chase to learn.

With that being said, I'd like to share a few of my key learnings from working on this project. Whether it be specific to JavaScript methods, any advice, or just a heads up on certain issues I came across. Hopefully anything I share from my experience can help those reading this save a few hours of going crazy (lol).

### Key Learnings:
#### 1. JavaScript Manifest
I came across a couple issues with my JavaScript loading when requiring them within my manifest file and soon learned that required files are loaded in alphabetical order unless you remove ```//= require_tree .```. So I did that, and added my JavaScript file (charities.js), by adding ```//= require charities```. That was one the first simple fix, but a good to know thing when starting your project! 

![](https://imgur.com/iCPB65M.png)

#### 2. alert or console.log
Another thing I learned, and definitely practiced a lot during this project is to ensure you're testing your click events before writing more code. Nothing is worse than writing out a whole block, and wondering why it's not working. The best part about this is that it's super simple. I like to add a simple ```alert('test')```, but when the pop-ups get annoying, I'll swap it for a simple ```console.log('test')```.

![](https://imgur.com/g6EbcPO.png)

#### 4. Prototype Functions
When creating prototype functions, it's best to create them as their own functions vs. within the consctructor function. The will still act the same way, and can still be called upon any instance of the class, but will not be created every time a new object is and therefore will save memory. You can call them as you need them. 

#### 5. Active Model Serializer
Learning about these within the curriculum was interesting, but really started to click when I got to generate my own and play with them. I highly suggest taking the time to add/remove attributes and associations to see what's being returned within your .json endpoint. I found this really interesting to see how easly it was to control what we wanted access to. 

## Final Thoughts
All in all, this project was definitely a challenge. I think more so because learning JavaScript is not very easy, especially when transitioning from Ruby and having to learn a completely different syntax. But building this really did help solidify a lot of the *huh* moments I had (and still continue to have!). Looking at JavaScript code and understanding it is a lot easier for me than thinking of how to write it. So if you're reading this and you feel overwhelmed or like it's just not clicking, know you're not alone! We all say it, that it's part of the process, and as silly as it sounds, it truly is! You're not expecting to learn it all in one section, but the more you practice, write, and break your code, the more you'll start to understand what's really happening on the other end of the text editor. 

Here's to hoping JavaScript and I can rebuild this friendship sooner than later, and until then.. I'm ready to meet React! 








