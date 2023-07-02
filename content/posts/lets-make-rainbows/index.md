+++
author = "Matt Lilley"
title = "Let's make rainbows 🌈"
date = "2023-06-30"
description = "I saw the most spectacular rainbow not long ago and wondered whether I could simulate it 🤔. I decided that, with the help of GPT, it would be totally doable and super fun."
tags = [
    "education",
    "science",
    "technology",
    "GPT"
]
subtitle="Creating digital rainbows with GPT4"
series = ["Let's make"]
+++

## Motivation

I saw the most spectacular rainbow earlier this year.

![Photo of a rainbow](rainbow-april-2023.jpg)

I should have been fully present in that moment (still working on that). However, I suddenly realised that, although have a physics PhD, I never really spent much time studying rainbows. I somehow managed to opt out of undergraduate optics classes which seems madness in hindsight. In my defense, I was doing a Maths & Physics course so something had to give 🤷‍♂️.

After the usual "pot of gold" ⚱️ jokes had been told and the spectacle faded into the clouds, I pondered on whether I could recreate this rainbow... inside my computer. In other words, could I simulate a rainbow?

The physics at play is well known - [refraction](https://en.wikipedia.org/wiki/Refraction), [dispersion](<https://en.wikipedia.org/wiki/Dispersion_(optics)>), [total internal reflection](https://en.wikipedia.org/wiki/Total_internal_reflection) - and we learnt about them all at school; so it should be simple right? I've made enough apps and simulations in my time to know it's never simple...ever!

And so, this lovely rainbow idea was consigned to the "Someday" page of my notes... that is, until I was emboldened by my recent success using GPT4 to help me create a [particle simulation]({{< relref "/posts/constrained-particles" >}}). After that, I was convinced that the rainbow idea was not only doable, but would be super fun.

## Result

2.5 weeks later, GPT and I finished making the first iteration of the interactive [Let's make rainbows app](https://mattlilley.com/lets-make-rainbows/). It allows you to explore the underlying
physics of rainbow formation by shooting light rays at various shaped prisms
and watching how the different colours bend and reflect. You can even make your
own shapes and also challenge yourself to traverse a "prism maze".

I think the app is fun, but of course it's not really "simulating a rainbow". It turns out the practical details are kind of complicated and so, as a first step, I decided to create something "simple" and not worry too much about the bits of physics that aren't quite right.

- reflection
- proper color mixing
- circle is not a circle
- light as a ray and not a wave
- exaggarated the different refractive indices of the colours

Despite the imperfections, my hope is that through experimentation people will develop a intuition for how light behaves and gain a deeper appreciation for the beauty of rainbows 🌈.

## The Process

Unlike my [constrained particles simulation]({{< relref "/posts/constrained-particles" >}}), which took me and GPT an afternoon to complete, "Let's make rainbows" took 2.5 weeks to build. Most of that time was not actually spent implementing the core physics. It only took a few days to start producing cool looking rainbow patterns with realistic refraction, dispersion and total total internal reflection like below:

<figure>
  <video controls src="tie-prism.mp4" style="width:100%"></video>
  <figcaption class="image-caption">100% reflective boundaries, 15x speed</figcaption>
</figure>

Instead, I spend a lot of time thinking about user expectations, their behaviour, differences between desktop and mobile experiences and testing. My past self was indeed correct "it's never simple...ever".

There is a huge gulf between making something work for you and making something work for other people. The process of taking an idea into "production" (even in a first iteration kind of way) requires you suspend all playfulness. You need (among other things) concrete ["user journeys"](https://en.wikipedia.org/wiki/User_journey), a robust user interface and you need to have anticipated the myriad ways in which your users might break all things 😣.

Now don't get me wrong, there is nothing wrong with the productionising process and it's rewarding to see an idea through to completion. However, every time I've made something "for production" I've always ended up feeling a bit flat afterwards. Perhaps this is just my way of working. I tend to treat everything as a sprint instead of a marathon and I have a habit of setting arbitrary deadlines and then working all the hours in order to meet them. By the end, I'm asking myself "Why am I doing this?" and "for fun" has kind of left the building by that point and I'm reduced to marvelling at my productivity/efficiency/agileness. For a project about 🌈 ... let's just say it's the wrong vibe 😂.

> Still writing...
