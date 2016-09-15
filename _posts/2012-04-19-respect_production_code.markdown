---
title: Respect Production Code
description: >
    Or "how I learned to stop worrying and love code that just works".
created: !!timestamp '2012-04-19 18:00:00'
tags:
    - development
---

It's part of our job, developers need to add different features to some code that is already running on a production system. It's just a matter of time before you find something you'd want just to throw away and rewrite completely. There are many possible reasons for this, I list a few of mine:

- The structure/style is out of date.
- The formatting is a mess.
- The code is messy and difficult to understand.
- Not many comments (in addition to the above).
- ... etc.

And yet, this is production code, and it doesn't contain so many bugs. How come? "It's incredible that someone even thought of putting such code in production! If I had my way..."

Yes, "if I had my way, I'd rewrite it completely". And maybe I'd need to rewrite or modify some of the supporting libraries, and also modify many other things during the process. And after wasting a ridiculous amount of time, we'd end up with a module that does the roughly the same as the old one, only with a new set of unknown bugs, for fun of the testing and maintenance people.

I admit sometimes I still feel this urge to reformat or rewrite code that is alright as it is, just for the sake of it. At least, after some years of being in the business, I already recognize it as a waste of time, unless it's useful for me or for people in the future.

I'm not saying it's bad to improve existing code, it's something that can and must be done, every time we have the opportunity. But it's important to pay respect to code that has already proven it can be run in production, and so all changes must be clearly improvements. If it's just a matter of personal taste, it's not worth to add an additional risk by trying to do "false refactorings" that lead you nowhere.

