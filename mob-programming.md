---
title: Lessons learnt from my first mob programming session
published: true
description: I will walk you through my journey introducing the idea of mob programming at work
tags: #mobprogramming #pairprogramming #productivity #teamwork
cover_image: https://cdn.pixabay.com/photo/2017/07/25/22/54/office-2539844_960_720.jpg
---
A few months ago, the YouTube recommender algorithm baited me with this presentation about Mob programming from Woody Zuill. 

[![Mob Programming](https://img.youtube.com/vi/28S4CVkYhWA/0.jpg)](https://www.youtube.com/watch?v=28S4CVkYhWA) 

It was the first time I heard about the term, hence I followed my curiosity and gave it a go.

**On this post, I am going to walk you through the steps I took to introduce mob programming to my team and what I learnt from it.**

# First impressions

Wikipedia says that Mob programming is:

> *Mob programming (informally mobbing) is a software development approach where the whole team works on the same thing, at the same time, in the same space, and at the same computer. [...]*

I’m sure you are thinking ...

![Thinking](https://media.giphy.com/media/DfSXiR60W9MVq/giphy.gif)

* How the **** can this be productive?
* If we don't even do pair programming at work, how can I convince my peers to try this?

That’s at least what I thought after watching the presentation 😅, so I moved on and a few months passed.

# Opportunity awaits

Fast forward to a week ago, my team was feeling pretty drained. We had been battling deadline after deadline for the past year, and it has been long since the last time we did something fun together.

This was the perfect moment to bring it up!

![Idea](https://media.giphy.com/media/3oz8xP6SaSkSU9dhcI/giphy.gif)

I knew everyone would jump on anything that would pull them away from work, but it couldn't be so long that it could raise some manager’s eyebrows. 

With that in mind, I booked a one hour meeting in everyone's calendar on a Friday and hoped for the best.

To my surprise, everyone loved the idea (even the managers 😮🎉). It was time to get to work.

# Preparation
## Mob programming agenda
> *The key to a successful learning environment is structure - Cara Carroll*

The first thing to figure out was the structure of the session. This would be a one hour trial, so I had to make sure I made the most out of the limited time.

I broke the hour down as follows:
* **10 minutes for introduction**. Where I would explain the dynamics of pair programming and the problem we were about to solve.
* **4x10 minutes blocks for problem solving**. This would ensure that a few of us would get a sense of what being a driver is.
* **10 minutes for discussion**. This would allow me to get a sense of what my peers thought of the experiment and understand whether this is something we want to try for real.

## Collaboration
> *Together we are stronger - Lots of people*

The next thing to define was how we were going to work **together**.

Again, because of the time constraint, I decided to play it safe on this one so that the tools wouldn't slow us down: **Git, Java, Maven.**

**During the session, the designated driver would periodically commit to the repository (always making sure that the build was passing before that) and, once they were ready to pass the baton, they would push to the repository.**

With that in mind, I created a repository with:
* A Maven project with 1 class and 1 test class.
* A README with a brief explanation on mob programming, a description of the structure of the session and a list of tools needed to take part.

After that was ready, I added a link to the repository to the meeting invite and shared in Slack, so that everyone could setup before the session.

In case you want to reuse something like this, I have pushed an example repository [here](https://github.com/albertowar/mob-programming).

## The problem
> *Wax on, wax off - Mr. Miyagi*

After a bit of browsing, I ran onto a site called [Katalyst](https://katalyst.codurance.com/) from [Codurance](https://codurance.com/) that has a ton of code [katas](https://en.wikipedia.org/wiki/Kata_(programming)) to practice the craft. 

I picked a problem called [String Calculator](https://katalyst.codurance.com/string-calculator). My intention was to keep the focus of the session around **getting familiar with mob programming**; therefore, I picked a simple problem that would not require a lot of brain cycles for experienced programmers.

![Secret](https://media.giphy.com/media/Yxg7MDkPj4kmI/giphy.gif)

We don't want people to start solving the problem in their heads and come with an idea on how to tackle it. We want to solve the problem **together**. Do not share the problem prior to the session.

# 3-2-1, action!
To ensure the session would go as expected, I played the role of a **facilitator in disguise.**

![Disguise](https://media.giphy.com/media/TWlXeBaWgWRWM/giphy.gif)

I was the first driver, so that everyone could see what that was about, and **continuously probed individuals for ideas** on how to continue. This helped us to get the ball rolling and encouraged everyone to be engaged.

Once my driver shift was over, I took a passive approach with small suggestions here and there but making sure that everyone would get their voices heard.

# Key takeaways
* **Onboarding**. I wanted to call this one out first because it caught me by surprise. We had a couple of engineers joining the team that week; and I noticed that it was the perfect way to show them how we code and what aspects we care about when improving code.
* **Bus factor → ∞**. With all the engineers working on the same code, the team is more resilient to attrition or people getting sick.
* **It was productive**. I wasn't expecting this one but, with a lot more 👀 on the code, we were able to fly through the kata and almost finish it by the end of the session.
* **Knowledge sharing**. One engineer was not familiar with the Java Stream syntax, and someone else explained how it works. Another engineer suggested using Regex to solve the problem, and everyone pitched in to discuss performance implications. This kept going spontaneously for the entire session.
* **Planted the seed**. Finally, the best takeaway was the fact that everyone started thinking about it. The next day, people already had ideas on how we could incorporate mob programming to specific areas of the next project to tackle 🥳. 



