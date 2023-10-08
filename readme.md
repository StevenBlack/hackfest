# Hackfest 2023

These are the notes for my [Hackfest 2023](https://hackfest.ca/) presentation.

The topic is presented in French. The title of the presentaton is "***Bitcoin: Cool et pas à peu près***" which is colloquial 
French for "***Bitcoin: Cool and not nearly***".  Which means, in essence, *Bitcoin is pretty cool*. The aim of the session 
is to explain Bitcoin while highlighting its cooler technical facets.

## Session outline

1. [Introduction](#Introduction)
1. [Epistemology of Bitcoin (some high level conclusions)](#Epistemology-of-Bitcoin-(some-high-level-conclusions))
1. [BTC, satoshis, and unit bias](#BTC,-satoshis,-and-unit-bias)
1. [Hashing, blocks, proof of work](#Hashing,-blocks,-proof-of-work)
1. [Block time, mining difficulty, and mining difficulty adjustments](#Block-time,-mining-difficulty,-and-mining-difficulty-adjustments)
1. [Bitcoin's heartbeat, and mining difficulty adjustments](#Bitcoin's-heartbeat,-and-mining-difficulty-adjustments)
1. [Halving and issuance](#Halving-and-issuance)


### Introduction

Here I extemporaneously explain who I am, why I'm here, and what I'm going to talk about. You had to be there.

### Epistemology of Bitcoin (some high level conclusions)

Why does it feel like explaining Bitcoin is so hard? It feels like
understanding Bitcoin has a high activation energy, with an elevated  "hump" that dissuades many people from understanding it.

![Activation energy](assets/endothermic-reaction.png)

If we list Bitcoin's salient subjects, and cross-reference among them for
prerequisite relationships, we get a table that looks like this.

![Base concepts and their prereqisite relationships](assets/base-concepts-related.png)

**All matrices can be represented as a graph network**. Here's the graph network of these prerequisite relationships. What a mess! Where to start 
to explain Bitcoin in a coherent way?

![Base concepts and their prereqisite relationships](assets/base-concepts-graph-1.png)

Let's use a **layered graph layout** to visualize the subject prerequisite relationships. This is a little better, but it's still a mess.

![Layered format for the network graph](assets/base-concepts-layered.png)

We can **analyze the network graph for cliques**. This is interesting because
it shows how some concepts are more tightly related.  This seems to be is a promising starting point for segmenting the subject matter.

![Cliques in the network graph](assets/base-concepts-cliques.png)

What if we score subjects for their prerequisite value, their complexity (the number of its prerequisites), and subtract prerequisite value from complexity score? 
This gives us a pretty nice roadmap! Let's cover the subjects thet unlock the most other subjects, and are least complex to begin with.

|   prerequisite (P)  | complexity (C)  | P - C  |
| ---- | ---- | ---- |
| ![](assets/scores-prerequisites.png) | ![](assets/scores-complexities.png) | ![](assets/scores-prerequisites-complexities.png) |

### BTC, satoshis, and unit bias

![8 decimals](assets/eight-decimals.png)

### Hashing, blocks, proof of work

### Block time, mining difficulty, and mining difficulty adjustments

### Bitcoin's heartbeat, and mining difficulty adjustments

### Halving and issuance

## Resources

These are links to things I referenced during the presentation.

- [The Animated Elliptic Curve](https://curves.xargs.org/)

- [Anders Brownworth's blockchain demo](https://github.com/anders94/blockchain-demo)

- [Clark Moody Bitcoin Dashboard](https://bitcoin.clarkmoody.com/)

