---
layout: post
author: Brady Boettcher
title: Paths in Music Technology
---

This post gives an overview of the music technology field (as of 2022) and explores some possible roles in professional and personal domains in the context of my own observations as a mid-level engineer in the field. I start by defining the field from different perspectives, and then reflect on paths taken by myself and close friends in music tech to help out those finding their own way.

For more about my own experiences, check out my [about me](/about) page.

---

## What is Music Technology?

As music technology implies the intersection of music and technology, let's explore the definition through the perspective of the musician (Music) and the engineer (Technology). Viewing the field of music technology as a spectrum between music and technology (Figure 1) may help those at either end to understand the bigger picture and where they might want to fit in. Each perspective has its own unique roles and skills that can be developed to virtuosity, and many more subdisciplines come forth when working somewhere in between. In this post, I've **bolded** the names of the roles as they emerge in the discussion.

<p align="center">
  <img src="/images/mt-spectrum-simple-dark.png" />
</p>
*Figure 1. A simplified spectrum of roles between music and technology.*

---

## The musician's perspective

Using technology to produce, perform and learn about music has been common practice for many years now, but is not required to get started in the industry. Acoustic instruments and performances still dominate much of the music we hear today, thanks to their recognizable sounds and styles developed over centuries. Advances in technology have enhanced much of the music recording, production, playback and distribution processes, leading to the creation of many new styles of music and performance. Let's begin our walk towards technology from the musician's perspective by first dividing musicianship disciplines into *composition*, *performance* and *education*.

### Composition

The affordances of technology for music composition are far beyond increasing the efficiency of transcribing notes onto sheet music. Digital composition has been transformed into music *production*, where all aspects of both acoustic and digital sounds can be intuitively recorded, edited and played back as a part of the creative process. **Music producers** manage a wide variety of skills including composition, sound design and mixing and mastering.

Audio synthesis and effect plugins (and hardware devices) can produce a number of new sounds and effects, and require their own set of skills to produce interesting results. **Sound designers** are the experts of controlling the parameters of synthesizers and effects to create new sounds or reproduce existing ones digitally. Newly created sounds can be distributed and bought/sold in the form of preset files, containing all of the sound's parameter values.

Mastering a music production program is a large undertaking that takes years, and that's not including the creativity required to produce good tunes. For this reason, **audio engineers** often act as technical operators for musicians that want to stay more on the music side of the spectrum. They must be able to translate the intents of the musician into quick results, which requires in-depth knowledge of music production tools. If the audio engineer isn't a sound designer, they must be able to easily find presets aligning with the musician's descriptions.

As you can probably tell by now, mastering all of these skills at once is extremely difficult for musicians, and this separation of disciplines is able to let musicians pick and choose which skills they want to develop using technology while leaving the rest to the experts.

### Performance

Technology offers many embellishments to musical performance, including new arrays of digital musical instruments (DMIs) and synced lights and visual systems for live shows. DMIs can capture complex gestures and map them to sound in ways not seen in acoustic instruments, although many aim to imitate gestures from acoustic instruments. Re-using known gestures can reduce the ease of access for new performers while providing unique sonic results. Visual systems are able to map to signals from the musical performance, taking many live performances to stunning new levels.

Many musicians are adopting digital instruments into their repertoire for both performance and composition. If designed well, these instruments can  be used to produce complex sounds with little knowledge of their technical workings. This is the job of **DMI designers** that create gestural controllers and synthesizers that provide new types of interactions for musical control. While gestural controllers produce control signals such as MIDI or OSC that can be turned into sound by external synthesizers, many DMI designers are tending to embed sound synthesis directly in the hardware itself (I plan on making a post about this trend in the near future). In order to create a digital instrument, DMI designers must be comfortable working with sensors, embedded systems and digital signal processing.

Arguably, the most important concept in DMI design is *mapping*, or the translation between gestures and the sounds that are produced (Figure 2). I might make a dedicated post to discuss this in more detail in the future, but [1] can function as a good starting point for anyone interested. For those wanting to get into instrument design themselves, I highly recommend checking out the NAMM and NIME conferences to see the cutting edge of the field. 

![](/images/mapping-diagram.png)
*Figure 2. A symbolic representation of a DMI from [1].*

Musicians can enhance their performances using projected visuals and lights that can be synced to interactions with input devices or the audio itself. Many professional performers work with **playback engineers** to customize all of the audiovisual aspects of their show. The above concept of mapping applies here as well when connecting signals from the performance to visual cues, and experienced playback engineers are able to carry out the mapping intents of the musician to create their ideal show.

### Education

The use of technology for music education lets newcomers find new methods to learn music theory, music history or how to play an instrument. **Music educators** create video tutorials, interactive applications, online courses or blogs like this one to provide valuable resources for musicians to learn many of the **bolded** skills in this post and more. 

---

## The engineer's perspective

Now that we've observed some paths for musicians getting into technology, let's discuss some opportunities for engineers to get involved in music. Using your engineering skills for musical projects can result in some great connections with musicians and other developers. The most important skill set to develop for this field is digital signal processing (DSP). DSP practices are at the heart of music technology, and can be used for audio *synthesis* and *analysis* to make some pretty incredible things.

### Synthesis

**Synthesis and effect developers** make devices that create and process sounds in complex ways, providing a set of parameters that can be controlled by the user. The interface to control the parameters is just as important as the processing capabilities of the device, and can be supported by the involvement of **graphic designers** in the project. In software, synthesizers and audio effects often come in the form of *plugins* that can be loaded into a music production program. Programming libraries exist for a few languages that support audio plugin development, but I recommend learning C++ and using [JUCE](https://juce.com/) if you plan on bringing anything to market. Your C++ knowledge will come in handy for learning DSP algorithms and finding jobs in this field too, so it's worth the effort to learn!

Another advantage of working in this field is the ability for independent developers to make a living on their own. Synthesis and effect plugins are relatively small and cheap projects to develop, and much of the code can be re-used between projects. Of course, this has also led to the oversaturation of the plugin industry, so your products really have to be something really special to convice users to buy them.

### Analysis

The field of music information retrieval (MIR) analyzes music and audio signals to extract features that be used for audio visualization, annotation and categorization. Many **MIR developers** work in research to publish their findings, while others use MIR as a tool in their musical projects to perform pitch and key detection, beat tracking and more. Machine learning is used for many MIR applications by virtue of its regression and categorization abilities, and I highly recommend checking out [The Sound of AI](https://thesoundofaiosr.github.io/) to learn and contribute to similar projects.

---

## Personal reflections

My own path began on the technology side of the spectrum with a computer engineering degree, but I've been able to work more towards the music side over the last few years. The biggest push to make this transition was the lack of creativity involved in traditional software engineering careers. I'd always enjoyed music production as a hobby, and many of my side projects were music related, but I always was pulled away from them due to the 40 hour work week that many of us know. Now that I'm back in school focusing on music technology full time, I'm confident that this is the field I want to work in. The community is worldwide spanning a myriad of disciplines, the work is hands on with plenty of creative freedom, and you're always a user of your own work.

I've talked to some friends about this concept of combining your hobbies with your career, but they almost always say that they would rather have a job unrelated to their hobbies in fear of passion turning into obligation. I think that this fear may hold true for some hobbies, but music technology offers an almost infinite creative space that evolves at a very rapid pace. If you get stuck in a job that isn't using your creative muscles, you can bet that there's some out there that will.

Unfortunately, careers between music and technology typically get more lucrative as you move towards the music side (Figure 3), which is why many find it easier to stay with a more secure, traditional job in technology and only pursue music as a hobby. I hope this post illuminates some of the possible paths in music technology that are available to help bring your musical hobbies to the forefront of your life. 

<p align="center">
  <img src="/images/mt-job-graph.png" />
</p>
*Figure 3. Job security on the music technology spectrum.*

---

## Conclusions

In this post, I presented the music technology field from both sides of the music and technology spectrum, discussed career paths that have emerged from it and reflected on my own path through it. I hope that people on either side of the spectrum have learned a bit about where they fit in now and where they might want to work towards. Thanks for reading, let me know if anything was unclear or needs revision!

---

## References
[1] Gibet, Sylvie & Marteau, Pierre-Francois. (2004). Gestural Control of Sound Synthesis. International Computer Music Conference Proceedings. 
