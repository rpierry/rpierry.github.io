---
layout: post
title:  "Distributed systems are complicated"
date:   2018-11-28
categories: technology, microservices
---

The microservices architectural style seems to be maintaining its position near the peak of inflated expectations along the [hype cycle][hype-link].  Some very large companies have had successes while utilizing this architectural style for parts of their business, which has fed the positive press.  This is all standard hype cycle stuff.  What should you and your company do about it?

As you consider embracing this style, it's important to keep in mind the [fallacies of distributed computing][distrib-link].  From a technical perspective, monoliths are strictly easier to deal with than microservices.  They are easier to debug, easier to reason about, easier to trace, easier to performance test, etc.  If your organization struggles to perform any of these tasks reliably on your monolith, microservices will not save you.

Why then do organizations consider converting their monoliths?  One explanation is the desire to solve organizational issues with technology.  When teams can't coordinate to ship a monolith, the idea of independently evolving and deployable services is quite appealing.  Instead of waiting for that other group to make and integrate their code changes, you can just deploy your service and be on your merry way.

Unfortunately, your organizational problems will still exist after an architectural shift.  Now, instead of these problems being very explicit and potentially delaying your build and release, they could become visible at runtime, when services don't adhere to agreed upon contracts or go down for inexplicable reasons.  If your organization lacks the maturity to monitor and consume services because this approach is new, the results can be catastrophic.  Moving to microservices trades compile/build errors for difficult to debug runtime errors.

Another draw of an architectural shift is the desire to jettison technical debt.  It's important to realize, though, that it isn't necessary to change architectural styles to accomplish this goal.  When organizations think about microservices, they are really thinking about a brand new system with no legacy baggage and then comparing it to their current systems.  The architectural style of the new system is immaterial to this comparison.  If technical debt really is weighing you down, there are many ways to remove it without turning a monolith into a more complex distributed system.

For example, a monolith designed with clear separation of concerns and a library-style approach to integration can decouple modules from each other without having to resort to distribution.  It's also a style that can be adopted piece-meal (just like microservices), allowing you to identify key capabilities, abstract them behind interfaces, and migrate usage to this new approach.

You can have automated builds, continuous integration, continuous deployment, and all the other trappings of modern systems with a monolithic approach, too.  

This doesn't mean that microservices are always the wrong approach, just that you should [do things on purpose][do-on-purpose-link].  Don't let the hype cycle distract you from being explicit about the problems you are trying to solve and whether or not an approach is truly a viable solution.


[hype-link]: https://en.wikipedia.org/wiki/Hype_cycle
[distrib-link]: https://en.wikipedia.org/wiki/Fallacies_of_distributed_computing
[do-on-purpose-link]: https://harmlessmachines.com/2018-07-09/do-things-on-purpose