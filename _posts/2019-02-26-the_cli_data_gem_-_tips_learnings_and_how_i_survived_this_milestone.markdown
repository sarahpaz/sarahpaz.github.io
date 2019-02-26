---
layout: post
title:      "The CLI Data Gem - Tips, Learnings, and How I Survived this Milestone"
date:       2019-02-26 01:28:25 -0500
permalink:  the_cli_data_gem_-_tips_learnings_and_how_i_survived_this_milestone
---

I gave myself a goal to complete the Object Oriented Ruby section of the curriculum before the end of February. After completing the last few labs, I thought - well, here we go - time to tackle my first portfolio project, the big CLI Data Gem. 

The first step into the land of portfolio projects can be quite scary. So before I get into the nitty gritty of my program, here are a few tips to keep you positive and help guide you through completing your CLI Data Gem.

**1. Plan!** 
It's a huge jump from labs to the project, and that was my rude awakening with this process. Tackling labs when you can see the amount of errors you've got to fix, with hints of what's missing is completely differenly than staring at a blank canvas and coding from scratch. I think I spent about 3 days planning how I wanted my CLI to work, the kind of interaction the user would have, the flow of the interaction, the classes etc. Out of those 3 days, I think I spent at least 1.5 days trying to find a good website to scrape.
**Takeaway:** Do not rush into the project, sit down, write out notes, and research websites. Figure out the ins and outs of how you'd like your program to work before diving into it. It'll help for a smoother process, I guarantee it. 

**2. Study Groups and Lecture Videos are Your New Best Friends!**
There are tons of study groups that will help you succeed! From practicing how you communicate your code, helping you prep, and to answering any questions or stucks you may have in the process. 
**Takeaway:** Not specific to this project, but to programming in general. It's time to step out of your comfort zone, ask for help when you need it, don't be shy, and don't be afraid to make a mistake. It's all part of the process! Take advantage of the amazing support Flatiron has to offer. 

**3. Pair Programming Works Wonders!**
Two heads are better than one! After staring at your code for so long, your eyes may let some syntax errors or typos slip. And in my case, the more I stared the more I started to forget what my code meant, or what I was doing! I partnered up with another student earlier in the program, and scheduled a pair programming session with her. It was very helpful for both of us, I'm sure! It's also a great way to continue to work on communicating your code. 
**Takeaway:** Put yourself out there on Slack, or reach out to other students you've met through study groups (this is how I met my pair programming partner!). Reiterating your code, or hearing someone else explain their understanding is a huge learning opportunity.

So, now the ins and outs of my CLI Gem. The website I chose to scrape is a tea website called [Tealish](https://tealish.com/). Here's a quick description on how my program interacts with the user:
* Greets the user
* Display menu of 3 tea flavors
* Display teas for flavor selected (first level scrape)
* Asks user to select a tea for more details (description, ingredients)
* Displays more details (second level scrape)

Another tip you'll learn from CLI lecture videos is to start off using [bundle gem](https://bundler.io/v2.0/man/bundle-gem.1.html) to generate your project skeleton. With this being your first project, it definitely helps hold your hand through getting the structure right! 

I started my project planning out the interaction:

```
puts "Welcome to Tealish!"
puts "Let's start by selecting a flavor collection."
puts "1. Fruity"
puts "2. Spicy"
puts "3. Floral"

```

Eventually breaking out this interaction into smaller instance methods within the CLI class:
```
class Tealish::CLI
  def start
    welcome 
    flavor_list
    menu
  end

  def welcome
    puts "Welcome to Tealish!"
  end 

  def flavor_list
    puts "Let's start by selecting a flavor collection."
    puts "1. Fruity"
    puts "2. Spicy"
    puts "3. Floral"
  end
end
```

Planning this way was very helpful, I was able to have my code laid out and see how I wanted everything to work, then break it down into separate methods responsible for specific tasks. 

That's one thing (of the many things!), I learned from Avi's videos on [Learn Instruct](http://instruction.learn.co/student/video_lectures#/). You should aim to have your CLI working and interacting with the user as intended before getting into the scraping. Use strings to fill in for your objects while you're getting the flow to work. Once all is as expected, you can tackle the more difficult tasks. 

All in all, it took me about 4 days to have my code "complete" (by complete, I mean functional), 3 days of planning, 1 days to refactor and create this blog post. I'd be lying if I said I didn't yell at my [rubber ducky](http://rubberduckdebugging.com/ family) (yes, I have 4) and dream about my code logic on multiple nights. This is no easy task, but you'll walk away with tons of learnings, feeling accomplished, and really seeing how much you've grown. You'd be surprised at how much you actuall know!

To end off, here are my top learnings after completing my CLI Data Gem:
* git commit, git commit, git commit!
* There's no shame in asking for help 
* Talk it out, to your friends, your cat, your dog, your rubber ducky, to anything! Hearing yourself explain your code will help you catch some errors.
* When you think you're done, you're not! There's always room to refactor! 

Good luck! You've got this! 

