+++
author = "Matt Lilley"
title = "Nuclear resonance energy transfer"
date = "2020-09-09"
tags = [
    "science"
]
subtitle="A Marie Curie fellowship proposal"
series = ["Solid state nuclear science"]
description= "The framing of nuclear fusion as a state transition draws our attention to physics where state transitions have been shown to undergo acceleration. A widely studied example is the transfer of energy between molecules of chlorophyll in close proximity inside plant cells"
toc = true
+++

The [Project Ida](https://www.project-ida.org/) team and I have been busy putting together a [Marie Curie fellowship application](https://marie-sklodowska-curie-actions.ec.europa.eu/funding?) for some solid state nuclear science research.

The process of applying for EU money is (as with many grant applications) very involved. It does however, provide a good opportunity to condense your thoughts and ideas into a coherent form.

If you're interested in seeing what the full application looks like, you can [download a copy here](Lilley-Marie-Curie-09092020-full.pdf).

If you're just interested in geeking out over the physics 🤓, then you'll find the relevant excerpts from the proposal below.

## Nuclear fusion rate enhancement by resonance energy transfer

### Project overview

Enhancing fusion rates could greatly simplify the extremely challenging engineering requirements for nuclear fusion. These challenges are rooted in the physical requirement for high kinetic energy of fusion reactants (which are typically hydrogen nuclei in plasma state) – and therefore high temperatures – believed to be inevitable for achieving substantial fusion rates. Without some form of enhancement, fusion rates are extremely low; for instance, fusion rates for D<sub>2</sub> molecules at room temperature have been estimated at about 10<sup>-64</sup>/s[^1]. In a high-density solid-state system, a rate around 10<sup>-20</sup>/s would begin to become technologically interesting. Fusion rate enhancements of about 15 orders of magnitude due to electron screening effects in solid-state environments have previously been demonstrated by Prof. Konrad Czerski[^2], as well as others[^3]<sup>,</sup>[^4]. For further enhancement, other mechanisms need to be considered. There are encouraging reports of substantial enhancement of state transition rates in quantum systems at the atomic scale due to couplings between resonant subsystems: Kaur et al. 2018[^5] report an 8 order of magnitude enhancement of transition rates in Rydberg atoms; Bang et al. 2019[^6] suggest that such enhancements can be further amplified due to the collective quantum effect of superradiance (as will be described below). If similar enhancement mechanisms can be shown to apply to the nuclear scale – as has been recently proposed[^7] and is indicated by related experiments[^8]<sup>,</sup>[^9] – then enhanced fusion in solid-state environments becomes technologically interesting. The overall objective of this project is to provide a sound theoretical and computational footing for such proposed quantum dynamics-based fusion rate enhancement mechanisms. Demonstrating alternative approaches to enhancing fusion rates – besides extreme temperatures – would loosen nuclear fusion engineering requirements, therefore helping fusion energy to become feasible sooner and possibly in cheaper form. Fusion energy in turn would represent a sustainable, clean, safe, yet affordable, stable, and highly scalable energy technology – technology features that today are highly sought after.

### Methodology

At the core of this project are the development and computational implementation of quantum mechanical models that capture the dynamics of coupled nuclei under realistic conditions. The starting place is an existing toy model that the author already implemented[^13] using Python’s QuTiP library and which exhibits expected features of excitation transfer and enhanced transitions between coupled subsystems. As part of the project, this model will be extended to match experimental conditions and results from experiments already conducted by a collaborating group at MIT (see references below). These experiments have been reported to exhibit phonon-mediated transfer of nuclear excitation in samples of coupled <sup>57</sup>Fe nuclei. After validating my extended model by comparing inputs and outputs with the experimental configuration, the model will be deployed to simulate behaviour (i.e. nuclear transition rates such as fusion rates) in a novel context (metal-hydrogen systems with candidate dopants as acceptor nuclei). The goal of this final part is to inform promising experimental configurations that can exhibit macroscopic effects from phonon-mediated nuclear fusion rate enhancement in solid-state environments (see below for details).


### Physics details

#### Nuclear fusion as a transition in a two-state system

Nobel laureate Julian Schwinger identified in 1991[^14] that the nuclear fusion process can be expressed in a typical framing of quantum electrodynamics (QED): a two-state system. For instance, the D+D → <sup>4</sup>He reaction is then viewed as a two-state system where the excited state |D<sub>2</sub>> in the form of a deuterium molecule can decay to a lower-energy ground state |<sup>4</sup>He> with the simultaneous release of 24 MeV of energy (from the mass defect). In Schwinger’s framing of the fusion process as a two-state system, where the fusion event represents a state transition, well-known toolsets of QED can be applied.

#### Accelerated transitions at the atomic scale
The framing of nuclear fusion as a state transition draws our attention to physics where state transitions have been shown to undergo acceleration. A widely studied example is the transfer of energy between molecules of chlorophyll in close proximity inside plant cells[^15]. Instead of a single excited chlorophyll molecule |e> transitioning to its ground state |g> on the nanosecond timescale, a coupled pair of molecules described by |e,g> (first excited, second ground) can transition to |g,e> (the excitation gets transferred) on the picosecond timescale without the radiation of photons. This radiationless process, known as resonance energy transfer (RET)[^16], has been known experimentally since 1922[^17] and has been placed on a firm QED footing since the 1980s[^18]. More recently, in experiments involving Rydberg atoms, state transition rates have been increased by several orders of magnitude[^19]. In these configurations, the RET processes – and therefore transition rates – are further enhanced due to a many-body quantum effect known as superradiance. Superradiance theory predicts that, when a large number of quantum states (N) is coherently excited, transition rates can be accelerated by a factor of N<sup>2</sup> [^20]. To evaluate whether such mechanisms also apply at the nuclear scale, what needs to be considered is the nature of the couplings between interacting molecules as well as the possible existence of alternative but comparable couplings at the nuclear scale. This will be discussed next.

#### Accelerated transitions at the nuclear scale

Searching for couplings similar to those that enable RET on the atomic scale would mean looking for electromagnetic couplings via the dipole/quadrupole moments of nuclei. These are the kinds of couplings that are exploited in Mössbauer spectroscopy to determine the chemical environment of nuclei in solids. Nucleus-nucleus couplings of this kind are however vanishingly small. When the dynamics of the lattice in which nuclei are embedded are considered, other possibilities come to sight. Since the 1930s, scientists have known that nucleon-nucleon interactions are momentum-dependent[^21] – which forms the basis of nuclear spin-orbit coupling[^22]. Although uniform motion affecting nucleons can be transformed away, the backwards and forwards motion characteristic of vibrational motion cannot. Such motion can then be thought of as a (weak) Lorentzian boost to existing spin-orbit splitting (a centre-of-mass momentum component that gets added to each nucleon’s relative momentum). Consequently, nuclear states can become weakly coupled with those of nearby nuclei through a coherent vibrational field (i.e. coherent phonons). In practice, theoretical estimates of such couplings are still small compared to nuclear transition energies but are nevertheless orders of magnitude larger than the well-known but miniscule dipole/quadrupole couplings[^23]. However, even small couplings are relevant in this context. This is because: (1) as shown in the RET literature[^24], even small couplings can enable transfer of comparatively large excitation in case of highly resonant states i.e. well-matched energy levels between donor and acceptor subsystems; and (2) couplings can be further amplified due to superradiance.

### Summary of objectives

The objectives of the proposed project include:

- Implementing the described computational quantum electrodynamics model with the goal of simulating realistic phonon-mediated RET events between atomic nuclei. The author has already implemented basic versions of such models (known as spin-boson type models)[^13] which need to be extended.
- Validating the computational model using the experimental conditions and outcomes from the described <sup>57</sup>Fe experiments[^25]<sup>,</sup>[^26].
- Application of the validated model to a novel context – rate enhancement of the fusion reaction D<sub>2</sub> → <sup>4</sup>He – and subsequent identification of promising experimentally accessible configurations from which macroscopically observable effects of fusion rate enhancement are expected.

The overarching objective of this research is to articulate realistic upper and lower bounds for the possibility of enhancing fusion rates via resonance energy transfer (RET) at the nuclear scale; and to identify experimental configurations that promise large versions of the effect, ideally large enough versions to become relevant for future technology development. As such, the proposed research seeks a transition from TRL 1 to TRL 2 on the Technology Readiness Level (TRL) scale.

[^1]: Koonin, S. E., & Nauenberg, M. (1989). Calculated fusion rates in isotopic hydrogen molecules. Nature, 339.
[^2]: Czerski, K., et al (2001). Enhancement of the electron screening effect for d+ d fusion reactions in metallic environments. EPL (Europhysics Letters), 54.
[^3]: Raiola, F., et al (2004). Enhanced electron screening in d (d, p) t for deuterated metals. The European Physical Journal A-Hadrons and Nuclei, 19.
[^4]: Schenkel, T., et al (2019). Investigation of light ion fusion reactions with plasma discharges. J. Appl. Phys., 126.
[^5]: Kaur, M., et al (2018). Dynamics of resonant energy transfer in one-dimensional chain of Rydberg atoms. The European Physical Journal D, 72.
[^6]: Bang, S., et al (2019). Superradiance and symmetry in resonant energy transfer. ArXiv Preprint ArXiv:1912.05892.
[^7]: Hagelstein, P. L., & Chaudhary, I. U. (2017). Coupling between the Center of Mass and Relative Degrees of Freedom in a Relativistic Quantum Composite and Applications. J. Cond. Mat. Nucl. Sci, 24.
[^8]: Metzler, F., et al (2018). Observation of non-exponential decay in X-ray and γ emission lines from Co-57. J. Cond. Mat. Nucl. Sci, 27.
[^9]: Chumakov, A. I., et al (2018). Superradiance of an ensemble of nuclei excited by a free electron laser. Nature Physics, 14.
[^10]: Dyson, F. (2013). “Six Cautionary Tales for Scientists” in From Eros to Gaia. Pantheon.
[^11]: See for instance Tennenbaum, J. (2020, April 27). Fusion power enters world of ‘extreme light.’ Asia Times. Waldrop, M. M. (2014). Alternative Fusion Technologies Heat Up. Scientific American.
[^12]: Call: H2020-EIC-FETPROACT-2019 (EIC Pathfinder: FET Proactive - Boosting emerging technologies).
[^13]: Lilley, M.K. (2020) “Excitation transfer” in Two State Quantum Systems. https://github.com/project-ida/two-state-quantum-systems/ 
[^14]: Schwinger, J. (1991). Nuclear Energy in an Atomic Lattice—Causal Order. Progress of Theoretical Physics, 85.
[^15]: Fassioli, F. (2014) Photosynthetic light harvesting: excitons and coherence. Journal of the Royal Society Interface 11.
[^16]: Jones, G. A (2019) Resonance Energy Transfer: From Fundamental Theory to Recent Applications. Frontiers in Physics, 7.
[^17]: Carlo, G. (1922) Über Entstehung wahrer Lichtabsorption undscheinbare Koppelung von Quantensprüngen. Z Phys. 10.
[^18]: Andrews D. L. (1989) A unified theory of radiative and radiationless molecular energy transfer. Chem Phys. 135.
[^19]: Brekke, E.G, (2009). Stimulated Emission Studies of Ultracold Rydberg Atoms, Thesis, University of Wisconsin-Madison. 
[^20]: Dicke, R.H. (1954). Coherence in Spontaneous Radiation Processes, Physical Review, 93.
[^21]: Breit, G. (1937). Approximately relativistic equations for nuclear particles. Physical Review, 51.
[^22]: Goeppert Mayer, M. (1950). Nuclear Configurations in the Spin-Orbit Coupling Model. I. Empirical Evidence. Physical Review, 78.
[^23]: Hagelstein, P. L. (2016). Quantum composites: A review, and new results for models for Condensed Matter Nuclear Science. J. Cond. Mat. Nucl. Sci, 20. 
[^24]: Andrews, D. L. (2009). Resonance energy transfer: Theoretical foundations and developing applications. SPIE Press: Washington.
[^25]: Metzler, F., Hagelstein, P., & Lu, S. (2018). Observation of non-exponential decay in X-ray and γ emission lines from Co-57. J. Cond. Mat. Nucl. Sci, 27. 
[^26]: Metzler, F. (2019). Experiments to Investigate Phonon-Nuclear Interactions (Thesis). Nuclear Science and Engineering Department, MIT, Mass.
[^27]: Lim, J., et al (2014). Phonon-induced dynamic resonance energy transfer. New Journal of Physics, 16.
[^28]: Pettit, R. M., et al (2019). An optical tweezer phonon laser. Nature Photonics, 13.
^[29]: Andrews, D. L. (2009). Resonance energy transfer: Theoretical foundations and developing applications. SPIE Press: Washington.
^[30]: Forbes S. (2019), Initial report on low-energy ion beam experiments with various metal targets [Conference presentation]. ICCF22, Assisi, Italy.