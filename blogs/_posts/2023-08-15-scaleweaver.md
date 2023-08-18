---
layout: post
author: Brady Boettcher
title: "A Pitch Interface Proposal: Scale Weaver"
---

This post lays out a proposal of a new pitch selection interface that I call Scale Weaver. It serves the purpose of providing an intuitive, easy-to-learn interface for playing music within a particular scale, while allowing the musician to naturally "weave" in and out of nearby scales during the performance.

### Quick terminology clear-up

In this post, when I write about pitch selection, I'm referring to the role of a musician to play a particular note on their instrument (e.g., holding a fret on a guitar, striking a piano key). I assume the 12 tone scale is the target of the musician, as it is the target of the proposed pitch selection interface.

## Why is this needed?

The main motivation for this project is to overcome my own struggle to master pitch selection on common instruments at the same level that I can accomplish it with my singing voice. *Mastery* is the goal of being able to quickly and accurately translate an imagined pitch into a played one. One of the ways this skill is often developed by musicians is with chromatic interval training, where two notes in the chromatic (12 tone) scale are played and the musician identifies the number of notes between them. While interval training is an extremely useful tool towards achieving pitch selection *mastery*, it usually requires an amount of additional translation between the target interval and the note to be selected, especially for non-isomorphic interfaces like the piano.

Isomorphic interfaces, which position intervals in a uniform pattern (e.g., the harmonic table, the linnstrument), get around this extra translation, yet the musician still must be proficient at recognizing chromatic intervals to play them easily.

The pitch selection interface I propose here further simplifies the interface to primarily feature notes in a particular scale. My hypothesis is that thinking in terms of scale intervals is more intuitive than chromatic intervals, and the interface also includes notes from nearby scales in order to retain flexibility and transition between scales.

Let's go a bit deeper into this concept of "nearby" scales and the *scale network*.

---

## Background

Dmitri Tymoczko's scale networks[^1] create an interconnected geometry of scales that achieve something called "maximally smooth voice leading"[^2] between connections. This means that in the scale network, connected scales each have only single note difference from each other. This achieves a natural continuity when modulating between scales in a performance, leading to the scale network being utilized in a number of composition tools. The network can be seen in Figure 1.

<img src="images/scaleNetworkLabels.png">
Figure 1. Dmitri Tymoczko's scale network visualized in [^3].

The tools that use this network have been primarily focused on analysis, generative composition and MIDI note filtering[^4] (to stay within a particular scale), but I have yet to see any applications of it for the purpose of a pitch selection interface. The interface I propose, Scale Weaver, keeps the precision of pitch selection seen in traditional instruments while making it much easier to play in a particular scale without memorization.

---

## Scale Weaver

The interface consists of a row of *main keys*, similar to the white keys of a piano. The main keys function dynamically depending on the current scale, repeating sequentially over all available keys. While Figure 2 shows a 1 octave version of the interface, it could be extended in either direction easily. Above the main keys are the *top keys*, which provide the voice leading notes to nearby scales in the network. As seen in Figure 2, only some of the main keys have top keys above them, which is a result of the number of nearby scales: diatonic scales each have 6 connections, while harmonic and acoustic scales have 4. Unfortunately, this results in not being able to play every chromatic note for harmonic and acoustic scales, and two pitches will be missing. Although, one could always navigate to the nearest diatonic scale and would have access to all 12 pitches if necessary.

To move between scales with Scale Weaver, my first idea is to have the user swipe a top key down to its main key to trigger the switch. All keys would then be updated to reflect the new scale, with only the top key that was swiped being the difference in the main key set. In this way, musicians can play within a scale and use voice leadings to hint towards a new scale, then switch into the new scale entirely and continue playing.

<img src="images/scaleWeaverDiagram.png">
Figure 2. A diagram of the Scale Weaver interface moving between three scales.

---

## Conclusions

This showcases the initial idea I have for Scale Weaver, and I'll be writing more about this as the work goes on. I've created a mockup Android app with this interface as a MIDI controller to try it out, and it felt natural and easy to play, which gives me confidence to continue with the experiments. Let me know if you have any thoughts about this at [bradyboettcher@gmail.com](mailto:bradyboettcher@gmail.com). Thanks for reading! :)

---

## References

[^1]: Tymoczko, Dmitri. "Scale networks and Debussy." Journal of Music Theory 48, no. 2 (2004): 219-294.

[^2]: Cohn, Richard. "Maximally smooth cycles, hexatonic systems, and the analysis of late-romantic triadic progressions." Music Analysis 15, no. 1 (1996): 9-40.

[^3]: Turczan, Nathan, Ajay Kapur, Nathan Ho, Colin Honigman, and Dexter Shepherd. "The scale navigator: A system for networked algorithmic harmony." In Proceedings of the International Conference on New Interfaces for Musical Expression. 2019.

[^4]: Nathan Turczan's Scale Navigator web app (and VST): https://scale-navigator-dashboard.vercel.app/about