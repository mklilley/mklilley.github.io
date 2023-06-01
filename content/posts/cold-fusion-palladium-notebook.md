+++
author = "Matt Lilley"
title = "Plotting Palladium"
date = "2020-01-24"
tags = [
    "science",
    "technology"
]
subtitle="Using Observable notebooks to aid research"
series = ["Cold fusion (LENR)"]
toc = true
+++

I'm currently involved in making my own cold fusion (LENR) experiments. For my experiments, I'm loading deuterium gas into a thin layer of palladium that's been deposited onto a nickel mesh and then heating the system to around 200C. 

No one knows how cold fusion works, and it seems to be very difficult to replicate. One parameter that appears to be important in the success of an experiment is what's called the "loading ratio" - the number of deuterium atoms compared to the number of palladium atoms. 

When the loading ratio is sufficiently high, palladium undergoes a "phase change" where the lattice expands significantly. In some theories of cold fusion, this expansion is necessary to create appropriate sized nano cracks in which a fusion event can occur.  Whether or not this idea is true, having a good idea of the loading ratio seems important.

In this post I've embedded an [Obvservable notebook](https://observablehq.com/) that I'm trying out as an easy way to visualise the loading I can expect during my experiments. 

You can find the original notebook [here](https://observablehq.com/@mklilley/deuterium-loading-of-palladium).

---

<div id="observablehq-03402c80"></div>
<p>Credit: <a href="https://observablehq.com/@mklilley/deuterium-loading-of-palladium@842">Deuterium loading of Palladium by Matthew Lilley</a></p>

<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@observablehq/inspector@5/dist/inspector.css">
<script type="module">
import {Runtime, Inspector} from "https://cdn.jsdelivr.net/npm/@observablehq/runtime@5/dist/runtime.js";
import define from "https://api.observablehq.com/@mklilley/deuterium-loading-of-palladium@842.js?v=3";
new Runtime().module(define, Inspector.into("#observablehq-03402c80"));
</script>