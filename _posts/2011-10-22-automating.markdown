---
title: Automating
description: >
    Or how I learned to stop worrying and love repetition.
created: !!timestamp '2011-10-22 10:00:00'
tags:
    - development
---

It's something you learn at any "Computers 101" class: Computers are supposed to be really good at performing the same task many times, right? Yes, of course, everybody knows that!

As everybody who works with computers knows that sometimes time is spent in really repetitive tasks, that should be automated somehow. And still, they aren't, and we keep repeating the same keystrokes and mouse movements. Maybe it consists of modifying several filenames one by one, or compiling different modules one by one in the necessary order over and over, or editing a long text file by copying-pasting-modifying...

I admit I still have a strong temptation to "exercise my fingers" when confronted to some tedious text-editing task (file editing, copying and pasting, etc.). I type quite fast, and sometimes it seems easier just to keep typing, than to stop and think for a while. You know, don't let some minutes of scripting spoil endless hours of typing fun...

And yet at the end, having the "how could I automate this" mindset helps you not only to save work, but also to avoid problems, not to mention again that it's "the right thing for computers to do".

Computers offer many ways of automating things, no matter which platform, operating system or IDE you are using. Taking the time to learn some of them and apply them in our daily job is really worth the effort.

For some years, especially when I'm developing, I have slowly grown accustomed to some interesting automation techniques that don't take too long to implement and always save me some tedious hours, and some equally tedious errors caused by some typo. They are __macros__, __automatic code generation__ and __one step build__.

I was supposed to know what a __macro__ was for, but the first time I understood their potential was many years ago, when my boss made magic with Emacs macros in front of me. Since then, every time I need to perform the same change in more than 10 lines of a text file, I ask myself if I should create my own Emacs temporary macro for it. I already know it can take shorter than doing it by hand. A more elaborate variation of macros are __refactoring tools__ (available in many IDEs), which remove some stress from my programming life by doing "the right thing".

Sometimes, __automatic code generation__ is already built in for your IDE, and it's easy to generate the skeleton of an application or a library. Sometimes, however, either there's no such help, or you need to create lots of similar skeletons, such as CRUD code for a web application. In that case, a small Perl script (or whatever scripting language of choice) can be really useful. It's not difficult to write, and if you I'm lucky sometimes I can reuse it in the future.

__One step build__ has been advocated [many times](http://www.joelonsoftware.com), so it shouldn't need many explanations. Once you get used to it (and there are tools like [Jenkins](http://jenkins-ci.org) that encourage you to), you don't want to get back to the times of "edit Makefile, copy this there, change this variable, run Make, open the IDE, change an option...".

Even if if might look a bit "geeky" at first ("hey, I wrote my own code generator!"), sometimes automation, in one way or another, is the way to go, just because it's what computers are supposed to be good at, and also because will save you time.

