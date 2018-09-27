---
layout: post
title:  "Inspiration and the end of Moore's Law"
date:   2018-09-26
categories: technology, agile
---

Informed opinion suggests that Moore's Law is coming to an end, or at least slowing down.  Though it's likely that we still have a few more ways to reduce feature size, these approaches are increasingly expensive and will eventually run up against the actual size of a single silicon atom or two.  Other materials may hold the answer, but these are conservatively a long way off.

Similarly, Dennard scaling is also over - smaller transistor sizes no longer mean a reduction in power required, in fact, now the opposite holds.

These were the two pieces of context [Pat Hanrahan][pat-link] used to kick off his keynote at [ICFP 2018][icfp-link].  Pat then observed that although this seems dire, there's cause for optimism, namely, the sorry state of the software and tools used to design processors.  

Because general purpose computers are hitting a performance wall, specialized architectures are a way to realize performance gains (think FPGAs and DSPs) at the cost of general applicability, but better tools are needed to make designing these domain specific architectures more feasible.  Because the current tooling isn't great, there are lots of gains to be made.

Pat's talk included much more than the above, including his work over the years to make this better tooling a reality, but an element underlying his point was the way he got here, first by bringing a physicist's eye to software and then by bringing a developer's eye to hardware design.  In some sense, this is a story of cross-discipline inspiration.

Cross-discipline inspiration and collaboration are hugely powerful tools, but organizational structure, tribalism, and mono-cultures often stifle them before they can take hold.  If you only have a single discipline within your company or people with the same backgrounds, fresh thinking is all the more unlikely.  If you teams don't value and respect the crafts of others, potentially interesting ideas will be dismissed outright.

You can find successful cross-pollination even within the disciplines used to make software.  Designers are demanding tools that let them approach design modularly, natively version artifacts, and transform a convenient representation for them to edit into something more suited for developers to consume directly after being exposed to and inspired by tools that developers take for granted like functions, source control, and compilers.  Developers advocate for designer inclusion and the time to really understand who we are building things for after being exposed to the capabilities and power of that craft. Even within development, front end developers are realizing that maybe those enterprise folks were on to something when they were talking about strong static typing when building large systems (and maybe those front end folks know a thing or two about collaborating at a massive scale to evolve tools at a blistering pace).

It's easier to highlight macro examples at a discipline level, but the same applies to the individuals on your teams who bring their own unique experiences and skills to the table.  [Software is made by people][people-link] after all.

[We][p202-link] believe in this enough to have made it core in our culture and methodology.  When you can simultaneously bring your beginner's mind to a new area while respecting the knowledge and experience of the people already working in it and they can mutually welcome your fresh perspective and enthusiasm, great things are possible.

[pat-link]: https://graphics.stanford.edu/~hanrahan/
[icfp-link]: https://conf.researchr.org/home/icfp-2018/
[people-link]: https://harmlessmachines.com/2018-05-01/software-is-made-by-people
[p202-link]: https://projekt202.com