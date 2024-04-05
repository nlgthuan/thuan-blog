+++
title = 'Thoughts on a workflow driven by AI'
date = 2024-04-05T20:41:49+07:00
draft = false
+++

> Senior developers without opinions tend to not be very good
>
> Junior developers with many opinions tend to not get good quickly (and are annoying AF)
>
> -- <cite>Boot.dev</cite>


When using AI to drive my daily work, usually, the feedback I receive is just sub-optimal solutions (not optimized, slightly wrong use of functions, bad design, etc…). It takes great expertise in the current language or framework to address these issues and and prevent the AI from steering in the wrong direction. Because this code just “works”, it’s challenging to detect the code smell.

When we try to produce mass code in a short time with AI, it is definitely harder to detect the code smell. Once the bad code gets into the codebase, the whole project get rotten quickly, just like [the broken window theory](https://www.freecodecamp.org/news/pragmatic-programmer-broken-windows-6916998eecbe/).


To me, working with AI is like working with a junior who knows a lot but can sometimes be annoying by not being humble and trying to make things up. You need to be really good at not letting it lead you in the wrong direction.


I believe that senior developers will benefit more from a AI driven workflow. But for junior developers or seniors when working with new languages, who have not yet been able to review code thoroughly, such workflow can cause more harm than help. We can never trust and learn from “a friend” who loves to make things up and tries to “gaslight” us all the time.


For example, last week, while I was working on the 1 Billion Rows Challenge (the post about this will be updated soon), in a language that I am not very proficient in (Golang, btw). When I tried to find a byte inside a bytes stream, I typed `bytes.I…`, Copilot quickly helped to fill in the rest with `bytes.Index(s, []{','})`, which worked perfectly.
If I weren’t curious enough to ask “why does it require an array of bytes as an argument, I just want to find a single byte”, I would never learn that the more efficient/suitable function `bytes.IndexByte` exists. And I had the same problem with `bytes.Split` and `bytes.SplitN` as well.
If I tried to reach to the document right away, I would have been able to go straight to the perfect solution at first try.
