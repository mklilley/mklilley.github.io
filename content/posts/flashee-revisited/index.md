+++
author = "Matt Lilley"
title = "Flashee revisited"
date = "2025-01-22"
description = "In 2018 I built a flashcard app called Flashee. But let's be real, the app wasn't very well written. In 2023 I decided to sort it out, and now it's 2025 lol."
subtitle="Refactoring with React"
tags = [
    "technology"
]
+++

Way back when, Christmas holidays of 2018 to be precise, I built a flashcard app called [Flashee](https://flashee.lilley.io/) because I thought that the flashcards apps out there sucked. I cleaned it up and made it available to everyone in 2020 and [wrote a blog post about it]({{< relref "/posts/flashee" >}}). But let's be real, the app wasn't very well written.

{{<image-link src="flashee.png" href="https://flashee.lilley.io/" alt="Flashee screenshot">}}

The code wasn't all that "clean"---it was a bit of a hot mess. Specifically, everything was in a single file...what was I thinking 😱! In 2023 I decided it was time to sort it out, and now it's 2025 🤣.

The refactoring was very start stop (mostly stop, e.g. I took a 15 month "break"), so, it took me almost 2 years to finish the job 😅. Although it took a long time, I averaged an hour a day on the 80 days I worked on it; I think that's pretty respectable for a side project. In terms of benefits, updates are going to be MUCH easier than when everything was in one file 😬.

I originally built Flashee using [Vue](https://vuejs.org/), but I decided to refactor the app in [React](https://react.dev/). The reason I chose React is that I'd recently finished teaching at a coding bootcamp and wanted to consolidate my React knowledge into a real project. I enjoyed getting into the weeds with React and would definitely use it again for other projects (especially when paired with [Vite](https://vite.dev/)). That being said, React has undergone all kinds of changes since 2023---sigh---so perhaps I'll need to take another look at the JavaScript landscape before I take on another project.... or maybe I'll just get ChatGPT to write it all for me 😆.

If you're interested in geeking out over how I built Flashee then you can find out more at the [Flashee Github repo](https://github.com/mklilley/flashee).
