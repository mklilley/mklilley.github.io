+++
author = "Matt Lilley"
title = "Two state quantum systems"
date = "2020-11-05"
tags = [
    "science"
]
subtitle="A model for solid state nuclear reactions"
series = ["Solid state nuclear science"]
description="The Project Ida team and I have created a series of computational tutorials in the form of Python-based Jupyter notebooks on two state quantum systems. Nobel laureate Julian Schwinger identified in 1991 that the nuclear fusion process can be expressed in a typical framing of quantum electrodynamics (QED): a two-state system."
toc = true
math=true
+++

## Reframing nuclear fusion reactions

A couple of months ago I posted some details about a recent [Marie Curie fellowship proposal]({{< relref "/posts/nuclear-ret" >}}) that I submitted. I can totally understand if you just glossed over it - it was a lot 😣. The most important piece of physics that's relevant to this post is:

> Nobel laureate Julian Schwinger identified in 1991 that the nuclear fusion process can be expressed in a typical framing of quantum electrodynamics (QED): a two-state system. For instance, the D+D → <sup>4</sup>He reaction is then viewed as a two-state system where the excited state |D<sub>2</sub>> in the form of a deuterium molecule can decay to a lower-energy ground state |<sup>4</sup>He> with the simultaneous release of 24 MeV of energy (from the mass defect). In Schwinger’s framing of the fusion process as a two-state system, where the fusion event represents a state transition, well-known toolsets of QED can be applied.

The typical framing of a nuclear fusion reaction is one of a deuteron tunnelling through the "coulomb barrier" presented to it by another deuteron [^1]. It's not obvious how quantum tunnelling is equivalent to the transitions of a two-state-system, as Julian Schwinger's describes. For now though, we're going to take Schwinger's lead and develop an understanding about two-state-systems and you're welcome to come along for the ride 😃.

## Two state systems (TSS)

The most common two state system discussed in introductory quantum mechanics courses is the spin of an electron. It was discovered experimentally, in [1922 by Stern and Gerlach](https://www.feynmanlectures.caltech.edu/II_35.html#Ch35-S2), that the spin of an electron along any direction is quantised, taking values of either $+\hbar/2$ or $-\hbar/2$. Although interesting in its own right, the mathematical description of spin has much broader applications - any two state problem can be translated into an equivalent spinning electron problem.

It turns out that the dynamics of some complicated systems can be approximately described by considering only two states. For example:

- [The ammonia molecule](https://www.feynmanlectures.caltech.edu/III_08.html#Ch8-S6) and the associated [ammonia maser](https://www.feynmanlectures.caltech.edu/III_09.html)
- [Molecular bonding](https://www.feynmanlectures.caltech.edu/III_10.html#Ch10-S1)
- [Nuclear forces](https://www.feynmanlectures.caltech.edu/III_10.html#Ch10-S2)
- [Photon polarization](https://www.feynmanlectures.caltech.edu/III_11.html#Ch11-S4)
- The decay of [strange particles](https://www.feynmanlectures.caltech.edu/III_11.html#Ch11-S5)
- Fusion of D+D → <sup>4</sup>He (if we believe Schwinger 😉)
- ... etc

The [Project Ida](https://www.project-ida.org/) team and I have created a series of computational tutorials in the form of Python-based Jupyter notebooks. The spirit of these tutorials is mainly towards demonstrating interesting quantum phenomena using the latest computational tools. To this end, we make significant use of a open-source python software called [QuTiP](https://qutip.org/) - huge thanks goes to their developers 🙏. 

You can find the tutorials on the [two-state-quantum-system Github repository](https://github.com/project-ida/two-state-quantum-systems) and if you're extra curious, you can see our peer review process for creating these tutorials by looking at the various pull requests, e.g. [this one](https://github.com/project-ida/two-state-quantum-systems/pull/17).


[^1]: [G. Gamow Zur Quantentheorie des Atomkernes Zeitschrift für Physik volume 51, pages 204–212(1928)](https://link.springer.com/article/10.1007/BF01343196), English translation [here](https://web.archive.org/web/20220327082154/http://web.ihep.su/dbserv/compas/src/gamow28/eng.pdf).

I hope you find these notebooks helpful. We'll continue to update them over time, so feel free to submit any feedback as a [Github issue](https://github.com/project-ida/two-state-quantum-systems/issues).