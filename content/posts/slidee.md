+++
author = "Matt Lilley"
title = "Slidee"
date = "2022-09-05"
description = "At its core, Slidee turns a folder of markdown files into Reveal.js presentations."
subtitle="A presentation tool powered by Reveal.js"
tags = [
    "technology"
]
+++

I've been working with web based presentation tools for years. Back in 2017, there were two main open-source tools for building beautiful web based presentations, [WebSlides](https://webslides.tv/) and [RevealJS](https://revealjs.com/). It wasn't obvious back then which one (if any) would survive to become the standard. Today, it is clear by comparing the project activity of [WebSlides](https://github.com/webslides/WebSlides/graphs/contributors) vs [RevealJS](https://github.com/hakimel/reveal.js/graphs/contributors) on Github, that RevealJS is the tool of choice.

I've worked a lot with WebSlides but often thought about making something with RevealJS. I always found getting started with RevealJS to be a pain. I wanted to be able to simply write some markdown like this:

```
<!-- contents of e.g. simple-presentation.md -->
Slide 1

### Notes:
A simple note for slide 1

---

Slide 2 

### Notes:
Some more structured notes
#### Point
The point of this slide 
#### Narrative
What I want to say on this slide 
#### Transition
How will I link to the next slide

---

Slide 3
```

 and then run something like an `npx` command to render that markdown as a beautiful RevealJS presentation. This didn't seem like an out of the box option, so I decided to build `Slidee`.

At its core, [Slidee](https://www.npmjs.com/package/slidee) turns a folder of markdown files into Reveal.js presentations. They look great out of the box, but can be styled to your hearts content. If that sounds like something you need in your life then you can find out more at the [Slidee Github repo](https://github.com/mklilley/slidee).
