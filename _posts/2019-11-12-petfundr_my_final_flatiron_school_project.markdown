---
layout: post
title:      "PetFundr: My Final Flatiron School Project"
date:       2019-11-12 06:39:26 +0000
permalink:  petfundr_my_final_flatiron_school_project
---


After almost a year in the online self-paced program, I've finally built my final project! In this post I'll briefly discuss what **PetFundr** is, what I learned about React functional vs. Class Components, and project planning tips.

### PetFundr: Raising Funds for Pet Medical Expenses
The idea behind my application is a "Go Fund Me" mock, focused on raising funds towards pet medical expenses. I wanted to build a clean design with a simple UI, and various features such as users being able to view all pets and make a donation, having the donation appear on their show page, as well as a progress bar on the pets show page to track progress towards the monetary goal. But as many project builds go, the original vision changed, and unfortunately I wasn't able to build this out exactly as I had planned. But, everything I did want has been added to a "Stretch Goals" list, and as I practice and continue to learn React and Redux, I'll continue to work at creating the app I originally envisioned. 

![PetFundr Home Page](https://i.imgur.com/mFxgZtL.png)

### React / Redux Learnings
Being honest, I came into this project feeling very unprepared. With that being said, a lot of what I learned about React and Redux really started to solidify as I was building this application more so than during the lessons/labs. So if you're coming into your project feeling lost, just know that's completely normal!

Here are a few learnings as I built this application, broken down very simply: 

#### 1. Functional vs. Class Components
In simple terms, the difference between functional vs. class components are that functional components are presentational (always renders the same information, based on the props). With functional components, you have direct access to *props*, where as with class components you access props through the use of *this.props*.

Below is an example of a functional component from my project used to display individual PetCards.

![functional component](https://i.imgur.com/mdEyKVz.png)


Class components are a bit more complex. They are able to have lifecycle methods and state, which allows the component to render differently.   

Below is a simple example of my HomePage component for my project build out as a class component. Notice the difference in the React import as well as the way the component is structured. Class components require the use of ```render()```.

![class component](https://i.imgur.com/kGXgydg.png)


Though there are clear differences in when to use functional vs. class components, if state or lifecycle methods are not a requirement, either component can be used. I personally prefer class components, as I've become more accustomed to writing them, but it really does come down to preference. Write what you're comfortable with! 

### Project Planning Tips
With this being my final project, I knew there would be a lot to plan out. I didn't expect it to take as long as it did though! Here are some key project planning takeaways that you may find helpful. 

#### 1. Brainstorm!
Don't limit yourself to your first idea. Brainstorm a few ideas, and try to plan out (e.g. write, draw etc.) the functionality, or how you want the application to work. Sometimes the first idea ends up either lacking requirements, or having too many features! Come up with a few ideas, and see which idea most easily hits all the project requirements. You can always add more features if you'd like after! 

#### 2. Prepare for your project planning meeting
Pick a couple of your top ideas (I had 2) ready to discuss in your project planning meeting. This helped me better visualize how everything would come to play with another pair of eyes (or ears), really understanding your thought process and helping iron out any unclear thoughts. 

#### 3. Visualize / mock up the user flow/functionality
This is something new I had to do with this specific project build. It may have been because it was my first React application, but drawing out where my routes would point to, which components would appear on each route, my containers, cards etc. really helped me get a clear visualization of the user flow. Even though I did deviate from the original mock ups, I would not have been able to plan functionality without seeing it all drawn out. There are tools online that you can use for this, a few I've looked into are [Lucid Chart](https://www.lucidchart.com) and [Mock Flow](https://www.mockflow.com/), but a good ol' pen a paper is what worked for me. 

#### 4. Create a dev log + requirements checklist
Organization is key with any project, and I found that with all my projects, creating a separate markdown file listing requirements really helped me stay on track. Marking them off as I'd complete them, for more transparency on my progress. This is also the first project where I created a dev log, and I think I'll be doing this for all future projects. Here I set daily goals, and would mark each goal off as I completed it. This kept me on focused on my projected goals for each day, and helped spot missing functionality or features that slipped my mind.


Most importantly, have fun! Enjoy what you're building, get excited about it! Sure, you'll get frustrated (a lot!), but you'll also learn a ton with each line of code you break. Whichever project build you're on, good luck!










