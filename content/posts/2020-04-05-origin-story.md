---
categories:
  - management
date: 2020-04-05
title: Origin Story
url: /2020/04/05/origin-story/
aliases: [
    "/management/2020/04/05/origin-story.html"
]
---


# Intent

My goal is to use this specific blog post to serve as both a starting point, and something I can refer to which describes the last three years of my career. Hopefully providing the reader with some context as to various decisions, cultural settings, and hurdles which helped define choices I have made and will make from here on out as I continue to add more content here.

As to why I have started a new blog in particular, I've been trying to come to terms with completely changing roles from an Individual Contributor (IC) to a Software Engineering Manager over these last few years. That includes things like breaking away from day to day programming, mentoring people, doing more project planning, administrative tasks, and constantly questioning whether I am acting like a proper force multiplier for my team. That last point is the most salient, because as an aspiring leader it's not as easy to define your career by your personal output anymore, and can lead to things like stress and depression.

A few resources which have helped me along the way that are worth mentioning up front:

- A large collection of engineering management resources on [GitHub](https://github.com/charlax/engineering-management)
  - Of which "Turn the Ship Around!", a book by David Marquet was immensely helpful
- An engineering manager focused blog by [Will Larson](https://lethain.com/) which I came across recently and is exactly the type of content I have been trying to discover for years now
- The support and blessing of my CTO to run my team as I see fit with absolutely no micro-management from him

# The Story

I lived in Japan from the years 2007-2018. Two were on the JET Program, the rest were a combination of Japanese mobile social game companies and consulting for other companies remotely, including the one I am at now. Part of me wants to brag about the cool stuff I was able to do at scale while working at some of these companies, however, the intent of this blog is to focus more on the leadership and management topics which surround tech rather than focus on any technical achievements themselves.

As it goes, the timing couldn't have been more perfect. As the 140 person game company I was working at as a Technical Lead started to tip a little sideways from the load of 4 over-budget and past-deadline projects, the CEO from AlasConnect at the time (of whom I've had a solid long term relationship with) asked me if I wanted to come back and run a brand new Software Engineering team. Without hesitation I said yes, with the caveat that it could be done remotely while I arrange visas for my family to move back stateside.

It helps to add context about the state of the company at the time. AlasConnect, a Managed Service Provider up in Alaska, had just been bought the year prior by our parent company. The goal as I understand it was to bolster their internal IT while we continue to provide and expand out to other businesses. There's no nice way to paint it though, there was a lot of bitterness and political fallout during this period as we inherited all of their IT employees, some of which were let go. I feel like writing negative things such as this could potentially detract from the content I write, but the truth is the world isn't all rainbows and unicorns. Sometimes what we build arises from the ashes of the previous iteration, and thus this serves as a dark yet important point for where things started when I came on board. 

After signing all of my paperwork stateside and meeting the members of my team, I was faced with running them remotely and at best with half-days given the timezone difference. The team was comprised of a few AlasConnect developers who were loosely building internal tools, and a handful of parent company developers who continued to write and maintain code in their work domain. Not one to pull punches: neither company had anything that resembled a modern day development culture.

# Building a Culture

In the startup world you typically start out with your founders who have built the initial product, and then they start hiring and scaling out their single product development team out as the business/funding increases. A large company likely has an established development culture, tools, and a pool of internal employees plus a hiring pipeline to fill out singular product teams.

That is not where I started. Instead, I was given a team of about 10 people from two different companies with varying backgrounds, including but not limited to experience levels, technology preferences, and projects they were siloed into. I had no clue how any of the vendor software, integrations, and custom software at our parent company (an ISP) worked. The AlasConnect developers were a fledgling group put together with the goal of expanding our software development capabilities, but no concrete plans or goals from high level management focused on the post-merger world. We were (and still are) distributed across 4 cities which introduces the unique problem of running a team in what is essentially a remote capacity. (After 18 months of US visa stuff I moved back to Alaska, and one of my guys moved to Chicago)

As a newly minted SE manager what were some core tasks I thought I should aim for? At the time I wasn't aware of the "first 90 days" concept, but the following is what I came up with.

- Meet with everyone and get an idea of who they are, learn what they are currently doing, and discover what they think the state of things are with regards to the big picture
- Discover what kind of software development principles have been put in place, if any
- Learn what the complex environment at parent company consists of, as it would be our primary focus for awhile
- Learn what the business goals of both companies are within the context of software development

What I discovered as I continued to talk with everyone, both developers and management, was that we needed to build a development culture from scratch.

- Technical
  - No core project management tooling, although JIRA had been introduced just before I came on
  - No central source control outside of the one or two projects myself and a colleague hacked on for AlasConnect and hosted on GitHub
  - No code review process since everyone was essentially siloed and this was never considered
  - No code testing, not surprisingly given a prior manager had said, "don't waste time on tests"
  - No CI/CD
  - A complete lack of logical dev/test/prod environments
- Interpersonal
  - Lack of 1on1s, feedback, and discussion about career growth (one time end year reviews only)
  - Group communication among team members was very low, which makes sense given the siloing
  - No real mentorship plans or long term personal goals
- Business
  - A distinct lack of documentation to help onboard new developers into existing systems
  - No communication loops with stakeholders, more of a top-down, "we need X so make it so" approach
- Misc
  - We had our very own Brent from the Phoenix Project that needed to have his knowledge disseminated

For better or for worse the Software Architect in me locked onto the idea that this was a chance to introduce something I was deeply passionate about, the Haskell programming language, something I have mentioned on our [company blog](https://www.alasconnect.com/2018/10/02/introducing-haskell-company/) a [couple times](https://www.alasconnect.com/2018/10/04/productive-haskell-enterprise/). As I sit here today I realize that was a very IC-oriented point of view which continues to haunt me with the questions, "Was it the right thing to do? Should I have pushed the choice down as a discussion and decision among the developers? Or was it more important to get people on the same page, even in a quirky language with a steep learning curve?"

Still, the technical stuff was actually quite easy to knock out as we weaved it through the large 24 month project we were handed, and made it to release with everything in place. I was also quite happy to have a motivated devops philosophist on my team who implemented a good chunk of what it took to make this work, his time and parallel understanding to my own was a boon with regards to moving us forward properly.

I have consistently started 1on1s late last year and they have been quite successful, especially with all of us working full remote from home due to the COVID-19 crisis currently. I was happy to see everyone jump in and mentor new folk as they cycled into our team, and it continues to be an enjoyable process for myself as well - likely one of my top favorite things to do. Our communication loops are a little tighter these days, and is an area we are constantly improving when we get the chance.

To this day the harder part has been the business side, something we continue to iterate on and refine. As our team becomes more focused on what our company calls "professional services", essentially consulting, we'll have an opportunity to introduce even more streamlined software development process into our culture.

# Accomplishments

Over the last three years we have released a few internal projects at both companies, assisted with improving existing software and business workflows, and above all fixed every bullet point in the above "technical" list leading to a dramatic change in the pace we can deliver to our parent company. Things such as new features mapped over older vendor systems, or helping integrate some of the myriad of customer focused products they have in the pipeline.

All of this culminated in the [release of our primary project](https://twitter.com/mojobojo/status/1232435697480396800), with happy management, shareholders, and developers alike.

And my own personal accomplishment, recognizing that I can no longer be a full time IC, but a proper team force multiplier. This still feels like an ongoing battle as I try to find a good balance between keeping my team-as-a-pipeline flowing and contributing in small but impactful technical ways when possible.

I hope that my dedication to becoming a better leader by continually trying to learn, experiment, and improve allows me to offer bigger and better chances for the members of my team to succeed, be it releasing new and exciting software products, or pushing their own careers in interesting directions.

I sincerely look forward to seeing what the future brings, and will make an attempt to document what I learn here.
