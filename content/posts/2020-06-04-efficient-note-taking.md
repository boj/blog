+++
title = "Efficient Note Taking"
author = ["Brian Jones"]
date = 2020-06-04
tags = ["management", "notes"]
categories = ["posts"]
url = "/2020/06/04/efficient-note-taking"
draft = false
+++

## Efficient Note Taking {#efficient-note-taking}

As my company starts belatedly revamping our corporate structure a lot of things have been changing, including my personal spiral towards a manager schedule vs a maker schedule lately. One thing I have noticed as I track more and more disparate things is that if I don't start taking better notes _now_ I'm going to fall behind and drown in forgotten caveats sooner than later. The less effective I am at tracking what I need to do (outside of task based work), or need to know across a breadth of projects, people, and responsibilities, the less effective I am going to be at supporting my team.

Over the last few months I've given a few note applications a look here and there. While my company has an o365 license allowing me to use OneNote, and it's not a bad product really, it didn't fit what I wanted. Part of my requirements are cross-platform, ideally allow me to easily export the data off the platform should I wish to, and above all give me a solid way to search and make sense of these notes over time. Perhaps a final little point that got tacked on was, "the more nerdy the better."

As I started hunting around for the holy grail I came across [Roam](https://roamresearch.com/), advertised as "a note taking tool for networked thought." Interesting. Unfortunately you have to request access at this time, and it appears it will be a paid, online, and likely vendor locked solution. Googling for alternatives lead me back to good ol' `org-mode`, and more interestingly [org-roam](https://org-roam.readthedocs.io/en/master/) which was released earlier this year.

-   Cross-platform? Sort of. Using [beorg](https://beorgapp.com/) along with [Working Copy](https://workingcopyapp.com/) on iOS is a decent solution for Apple mobile. Can sync a git repo to iCloud with Working Copy and then point beorg at that folder.
-   Export data? Absolutely. Full control over my `org` files, stored in git, and synced with whatever platform I want.
-   Search? Yes! Not only does org-roam do bidirectional linking, which is really its biggest selling point, if you add `daft` as a way to search through your notes it's a concrete method.
-   Nerdy? It's emacs, so of course! I'm giving [doom-emacs](https://github.com/hlissner/doom-emacs) a shot this time over [spacemacs](https://www.spacemacs.org/) for configuration. (I still code with [kakoune](https://kakoune.org/) when I have the time, the movements are more intuitive than vim to me)

For the super curious there is [this blog post](https://zettelkasten.de/) about a concept called Zettelkasten, a particular way to not only do note taking, but conceptually think about note taking. I'm still trying to soak it in, however, it really resonates with me so far.


## Workflow {#workflow}

Part of what makes this a good note taking method is the workflow. There are a couple things `org-mode` has to offer which help me out on a daily basis. The bulk of the important note taking comes from using `org-roam` methodologies.


### Process {#process}

I think it's useful to describe the process before the mechanics.

`org-roam` prescribes a non-nested folder structure, which aligns with this idea that you don't build hierarchical structure, instead you deeply associate things through heavy use of links. So I have a local directory at $HOME/.org/roam where I store everything in per-topic org files. These could be anything from this blog as `blog.bojo.wtf`, `2020 Journal` for "fleeting thoughts", `John Doe 1on1` for notes and goal tracking of an employee, to `Org Roam Notes` and `Books` to keep track of tidbits and interests. The actual file ends up looking something like:  $HOME/.org/roam/20200601082030-blog\_bojo\_wtf.org

At the end of the day, regardless of the state of any mid-process notes, I commit the data to git with a commit message corresponding with the day in order to keep it synced. (I forgot how awesome [magit](https://magit.vc/) is!)

And that's basically it.


### `org-journal` {#org-journal}

I am using a yearly [org-journal](https://github.com/bastibe/org-journal) file to track meetings, including time entries, `org-mode` tags, and relevant notes in a structured subtree. I create `org-agenda` TODO tags to help keep my eye on things I need to actively participate in by pulling up Org Agenda.

```org
 #+TITLE: 2020 Journal
 * Wednesday, 06/03/2020
 :PROPERTIES:
 :CREATED:  20200603
 :END:
 ** 08:30 Standup Meeting :internal:standup:meeting:
 ** 09:00 Weekly Admin Meeting :internal:admin:meeting:
  - Person A will sync up with Person B about the Product stuff
  - At some point we need to work out a data warehouse schema
 *** TODO Meet up with Person C and discuss data warehouse tooling
```


### `org-roam` {#org-roam}

Probably the coolest thing I've done recently was convert this blog over to [ox-hugo](https://ox-hugo.scripter.co/) (and from jekyll to hugo) and start maintaining it all in a single `org-roam` file.

Tracking 1on1s is proving useful, especially as I continue to refine my note taking around these meetings. I realized at some point that it's a disservice to my employee by not taking notes for things I need to actively be thinking about, organizing, or helping with, because there is a chance it falls through the cracks of my aging mind. Long term this helps with our yearly performance reviews (an unfortunate point which hopefully changes, yearly is not enough), and will serve as a nice paper trail to give more concrete documentation.

Everything else revolves around notes about work, hobbies, personal interests, and references.


## Final Thoughts {#final-thoughts}

This is still a process. Until I get a few more weeks/months of deeply linked notes the gains aren't making themselves clear yet, however, I suspect that by simply forcing myself to take notes about everything this is going to help with my long term productivity.
