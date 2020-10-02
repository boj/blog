+++
title = "Effective Time Slicing"
author = ["Brian Jones"]
date = 2020-10-01
tags = ["management", "leadership", "time"]
categories = ["posts"]
url = "/2020/10/01/effective-time-slicing"
draft = false
+++

## The Problem {#the-problem}

When you ask someone on your team to spend 20% of their time working on another task, what happens? Do they effectively break their day/week/month down? Do you have to step in? Is the task done properly and to spec?

What I have observed directly in the wild is that they will spend Monday through Thursday working on their primary task, and then allocate Friday for the 20% time asked of them for the secondary task. The reality of the situation is that their primary task bleeds into Friday, and the secondary task gets pushed back to the next week, and so on, usually due to the perceived importance of their primary project.

Worse, the required throughput for the secondary task falls behind, and the end result isn't as solid as it could have been if the time was more effectively managed. Still, as managers we aren't interested in micro-managing our employee's time, are we?

What can we do to fix this?


## Use Case {#use-case}

My Software Architect has a solid end-to-end infrastructure, CI/CD pipeline, and process in place with which we use to deliver a half dozen products and several dozen system components for a few companies and projects. We've reached a point where it's not efficient for him to be the sole proprietor of these systems, a problem we have been working on solving for awhile now (my own personal mandate is to de-silo <span class="underline">everyone</span>, build redundancy into the team, and spread the knowledge).

In order to achieve this I have explicitly asked my two Senior Engineers to spend at least 20% of their week taking the time to do the training, testing, and implementation work required to get up to speed with our Architect. As one might guess, they haven't been able to properly spread their time out in a way where they feel like they are effectively achieving their goal, and have expressed the fact that they don't feel like they are making genuine progress. Why is this?

After a couple conversations we came up with a few points:

-   As stated earlier, the perceived importance of their primary task was taking priority in their minds and not allowing them to back off and make time for the secondary task
-   Even though I emphasized the importance of the secondary task, it turns out saying "use 20% of your time" is quite arbitrary and not enough to properly get them into the right mindset
-   If there was structured training with the Architect things were progressing, however, self study and dedicating time to the task solo were harder to get measurable results from


## A Solution {#a-solution}

Because Individual Contributors are focused on their tasks on a day to day scale, I propose that it then makes sense to frame the time scale for additional tasks around the unit of a single day.

If we propose they spend 20% of their time to a secondary task, then that means they should instead dedicate two contiguous hours <span class="underline">each day</span> for that task.

This achieves a few goals:

-   They now have a structured schedule with dedicated time to focus on their task
-   They have their manager's blessing and support to spend this time on that task, removing any worries about not performing on the primary task
-   Due to having a consistent schedule the task can now be achieved in a reasonable amount of time, and without cutting corners


## Taking it Further {#taking-it-further}

One day one I asked my boss to treat my team as a pipeline. We're not a single product software shop, instead we are closer to a consultancy with which the bulk of the work is for two internal customers from different companies. This means we have a large amount of new projects coming in, older projects to support and maintain, and even older projects to sunset and kill off. There is no sane way to keep up with that work without designing a capacity level around your team(s).

What I have done here is two-fold:

-   The entire department has a capacity value of 100%, which if tracked properly in a rubric of people/project percentages
    -   This allows me to say the magic word "No" when we are at absolute capacity
-   At the _individual_ level I have assigned only 90% capacity to each person

The interesting part here is the individual level. Where did that extra 10% go? Meetings, covering people who are out, ad-hoc discussions, personal learning and improvement time, etc.

In practice this method appears to make my team happier, because their goals are more manageable and concrete. A happy team means increased productivity, more throughput, and people that enjoy coming back to their desk day after day to hack on new and interesting things.
