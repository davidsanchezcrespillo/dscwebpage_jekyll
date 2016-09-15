---
title: Dependency Injection in practice
description: >
    Or "how I learned to stop worrying and love Dependency Injection".
created: !!timestamp '2012-03-30 18:00:00'
tags:
    - development
    - patterns
---

The first time I heard about [Dependency Injection](http://en.wikipedia.org/wiki/Dependency_Injection), I thought it was a nice concept, but difficult to implement in practice. However, as I started to use it for some projects, I discovered it has some advantages that make it worth the effort to learn, and it isn't so difficult to implement after all.

What's the __main principle__ of Dependency Injection? Actually, it's quite simple: When your object needs to call another object, it gets it from the "outside world", instead of creating it itself. In practice, this means "no _new_ statements all around your code".

So, instead of this:

    class MyClass {
        Member member;
            constructor()
        {
            member = new Member();
        }
    }

you would write this:

    class MyClass {
        Member member;
        constructor(Member inputMember)
        {
            member = inputMember;
        }
    }

(You don't actually need to pass your objects in the constructor, you can do it in any method you wish). 

Where do the objects get created, then? Ideally, in a specialized class, devoted only to this task. This class (let's call it __container__) can also manage the dependencies between objects (so, "this object A needs this object B, and it's passed through this method"). Sometimes, objects are called "services", which reflects much better their intent.

Should I write a container, then? Well, if you wish, that's OK. However, there are Dependency Injection Frameworks ready to use, in all the major languages. [Spring](http://www.springsource.com/developer/spring) and [Guice](http://code.google.com/p/google-guice/) for Java, [Symfony DI](http://symfony.com/doc/current/components/dependency_injection.html) or [Pimple](http://pimple.sensiolabs.org) for PHP, etc.

After using a bit Dependency Injection for some time now, I have found the following __advantages__:

- Centralization of the object creation responsibilities into a single class. You don't write _new_ statements everywhere in your code, but only inside your Dependency Injection container.
- Efficiency (if your container uses lazy evaluation). You can instantiate your objects only when they are needed, and even share some of them, without creating them every time, or maintaining global information (the less global information you maintain, the better).
- Testability. Since you pass the dependencies "from outside" to each object, it's much easier to use mock objects and stubs without modifying the code you are going to test.
- Better design and programming discipline from the beginning. If you have started using dependency injection, you'll soon be using it everywhere as a habit. Also, because you need to declare explicitly the relationships in your object tree, you'll be able to detect possible circular dependency issues more easily.

It sounds nice, but of course it doesn't come for free. Which additional __effort__ did I need to make? Of course, I needed to learn how to use my container of choice, and also to structure my code accordingly. The main tasks I had to perform were the following:

- I had to replace a bunch of _new_ operator calls in my code. Of course, it's not feasible to try to put Dependency Injection into your "big old application" all of a sudden, replacing working code with that "new fancy stuff". Instead, I started refactoring a subset of objects, leaving other parts for later. The benefits listed above were immediately visible.
- Every time a new class was added to my program, I needed to consciously place it inside the dependency tree, so that it could be created properly. This gave me some headache, when some hidden circular dependencies were revealed between some of my classes. It was good, however, to be able to detect them as early as possible.

In short, I needed to "play according to the Dependency Injection rules", to be able to get some benefits in my code (I personally appreciate testability most of all, no more scratching your head thinking how to write a unit test for that huge class containing dozens of internal references to other objects). Like with any new discipline, you need to start at a slow pace, but as you keep working, you speed up, and it's not difficult to get used to it quickly.

