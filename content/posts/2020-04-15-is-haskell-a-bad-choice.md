+++
title = "Is Haskell a Bad Choice?"
author = ["Brian Jones"]
date = 2020-04-15
aliases = ["/management/2020/04/15/is-haskell-a-bad-choice.html"]
tags = ["management", "leadership", "haskell"]
categories = ["posts"]
url = "/2020/04/15/is-haskell-a-bad-choice/"
draft = false
+++

## Quick Note {#quick-note}

To save you some time I will give some reasons to immediately close this tab in your browser.

-   This post is about making a management decision to use Haskell
-   This post is not about any technical accomplishments with Haskell
-   This post does not actually conclude that Haskell is a bad choice

Otherwise, I hope what I have laid out below serves as a good view into a non-software company up in Alaska using Haskell to develop applications with.


## Prelude {#prelude}

Recently I [stated on Twitter](https://twitter.com/mojobojo/status/1250137071164854272) that I hadn't written a Haskell blog post in 3+ years. In my mind I was going to write a large number of these which described the myriad of amazing problems my team solved with the language, guides to help newcomers to the language, and maybe even talk about libraries we had contributed back to the ecosystem. The desire is still there, but perhaps my view has warped more towards what _business needs_ it solves, rather than what interesting _technical solutions_ one can actually achieve with the language.

In my [Origin Story]({{< relref "2020-04-05-origin-story" >}}) post I laid out the basics for what got me where I am today. The particular point I want to focus on in this post was whether or not I felt, and continue to feel, that adopting Haskell with my team was a good idea _from the perspective of a leader_. Along side this core question I hope to present some anecdotes which show what I have encountered while taking a team of never-used-Haskell-before imperative programmers from novices to advanced users of the language.

> Was it the right thing to do? Should I have pushed the choice down as a discussion and decision among the developers? Or was it more important to get people on the same page, even in a quirky language with a steep learning curve?

To this very day these questions haunt me.


## Haskell Shops {#haskell-shops}

What kind of Haskell team compositions do we typically see out there? I ask this question because it's important to add contrast between "what is typically normal" vs "what **I** ended up with."

-   Haskell consultancies: On average these seem to be driven by high level academics capable of taking their technical acumen and applying it to the business needs of others using Haskell.
-   Haskell startups, teams: These are companies, or teams embedded in larger companies, which have the opportunity to hire Haskell developers immediately due to it being their core competency.
-   Lone Wolf: This comes up in [r/haskell](https://www.reddit.com/r/haskell/) on occasion. Usually someone trying to discover a solid way to introduce the language to their team from a position of little power. I've [offered feedback](https://www.reddit.com/r/haskell/comments/9kafdv/how%5Fto%5Fintroduce%5Fhaskell%5Fin%5Fa%5Fwebdev%5Fshop/e6xoxav/) at times with the hopes that they were able to move forward with that advice.

The contrast comes from the first two examples, which is the fact that those companies are able to hire motivated Haskell talent from day 1.

-   People passionate about the language
-   People that want to solve interesting problems using the language
-   People that see the power behind using such a language

Note that I am not implying that hiring Haskell developers is hard! I am merely setting the stage for how my own team got to where they are today. No one on my team remotely touched any of those points, which makes introducing Haskell a quirky problem.


## Introducing Haskell {#introducing-haskell}

Up to this point I have trained about 12 developers into Haskell over the last 3+ years, of which a few were new hires, and the rest were developers who were at the two companies prior to me getting hired. The most exposure to Haskell any may have had was through a Programming Languages course they took at university.

The parent company team was using C# to solve problems. My company's team was doing a bit of exploration with Elixir. I showed up on the scene with the blessing of our CTO to train them all into Haskell, even if it meant longer than usual bootstrapping time compared to other commonly used programming languages.

In the beginning it seemed prudent to keep a 50/50 split between the two companies and teams. The C# guys would continue on as they had been, and the rest of us would explore Haskell and use it as a starting point to tackle internal tooling. Our teams would then meet in the middle when it came to code management, deployment, and modern day best practices.

As it goes, we lost one of the parent company developers shortly after due to the fallout from the company merger. We lost another a few months later, right as that team was about to start working on a critical project. By this point the project did not have enough developers to be successful, so my CTO recommended that we go all hands on deck.

Except no one from my company wanted to write C#.

I declared that we would be writing the new project in Haskell.

And at this point in the story we discuss whether it was a proper leadership decision.


## Question Thyself {#question-thyself}

> Was it the right thing to do?

As a manager new to the team who is supposed to lead existing developers across two companies and mixed toolsets, was it prudent to make them all learn a language which is notorious for being difficult to grasp? Even if the long term promises of the language are a worthy goal? I should note that part of the problem here was that I had not yet learned that I was no longer an IC, and was jumping in and injecting my opinions, where in hindsight maybe I should have not.

Pros:

-   The entire team is now using the same language for everything, less any legacy projects
-   The entire team now rises and sinks together via shared expertise
-   The long term benefits of using this particular language, specifically how type safety makes it easier to modify other people's code without fear

Cons:

-   Unhappy C# developers who had been satisfied with the .NET ecosystem
-   An average 1-3 month ramp up time into Haskell depending on experience and temperament. Roughly a year to feel like they really _get it_
-   Discovering proper language methodologies, libraries, and idioms across the whole team took much longer than anticipated

Although to be fair, that last point has been a great experience, even though I list it as a con. The reason it is a con, though, is because a team full of experienced Haskell developers wouldn't have had to spend as much time as we did doing discovery.

> Should I have pushed the choice down as a discussion and decision among the developers?

This is the one I keep coming back to. Was it a good leadership decision to dictate the tool everyone would be using? Perhaps I should have given the people writing code in the trenches the proper time to research and vet a set of tools they would have all been happy using, or at the very least feel like they had a say in.

Pros:

-   Team is included in the decision making process about tools they themselves have to use on a daily basis

That's a lonely little bullet point, but it's all I can come up with. Being inclusive is important to me, even though I did not do it in this particular case.

Cons:

-   How many different languages would they have explored? More Elixir? Go? Would the C# team be adamant that we adopt their tools?
-   How long would this process have ended up taking? I'm not sure how to actually measure that because I have never done it.
-   The critical project we were supposed to be tackling at that point would have gotten pushed back further as we did even more research and discovery

I'm curious if the people driving the conversation would have been as heavily motivated as I was to push Haskell? There's a lot of passionate programming language enthusiasts out there, but we don't seem to have any of those on my team with the exception of myself. Perhaps this is a good thing, since it means they care more about the product than the tool they use to ship it.


## Guidance {#guidance}

What I quickly discovered was that no one was going to just sit down and start experimenting with random Haskell code.

-   I wrote up a slide deck and presented it, and built a large list of existing online resources as reading material
-   I bought them some Haskell books which helped bootstrap their minds into the mindset it takes to use the language, but they completely fall flat with guiding a developer towards how to be productive with the language in an industrial setting

These are great if you have people motivated to use the language right out the door. It turns out you need to do more if you have a team full of skeptics.

-   I wrote the original starting code for the primary project we were going to hack on which served as a template for everyone else to examine and build off of
-   I did a lot more pair programming to help ease people into understanding what was going on with the code
-   Code reviews were necessary to make sure people were following the style guidelines and not going too far into the weeds

Those final points ended up being the most effective.

Most importantly, what helped in the long run was the support of my two senior developers from my company. After getting some working examples into their hands they quickly started to see the value of Haskell, and helped me promote it to the rest of the team. Without their support I'm not so sure this would have been a successful endeavor.


## Conclusion {#conclusion}

It turns out that my team [released that critical project](https://twitter.com/mojobojo/status/1232435697480396800) a couple months ago and are even beginning to take a good hard look at how to introduce even more [type safety](https://twitter.com/mojobojo/status/1243654057056555008) into our applications. Perhaps getting a group of former imperative programmers into a purely functional language mindset wasn't so hard after all.

Even though I personally still struggle with this ancient decision, it seems my team has actually moved past this and are continuing to hack in Haskell every day with no complaints. One of my C# developers still drops a comment like, "the .NET world has already solved this problem" on occasion, but then he turns around and shows the whole team how to properly use `TypeFamilies` and why it applies to `servant` library types.

Given our success, I am firmly going to say that, no, Haskell is _not_ a bad choice!
