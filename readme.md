# Hackfest 2023

These are the notes for my [Hackfest 2023](https://hackfest.ca/) presentation.

The topic is presented in French. The title of the presentaton is "***Bitcoin: Cool et pas à peu près***" which is colloquial 
French for "***Bitcoin: Cool and not nearly***".  Which means, in essence, *Bitcoin is pretty cool*. 

The aim of the session is to explain Bitcoin while highlighting its cooler technical facets. In 45 minutes.

## Session outline

1. [Introduction](#Introduction)
1. [Epistemology of Bitcoin (some high level conclusions)](#link-to-come)
1. [BTC, satoshis, and unit bias](#link-to-come)
1. [Hashing, blocks, proof of work, and mining](#link-to-come)
1. [Bitcoin's heartbeat: Block time, mining difficulty, and mining difficulty adjustments](#link-to-come)
1. [Halving and issuance](#link-to-come)


### Introduction

Here I extemporaneously explain who I am, why I'm here, and what I'm going to talk about. You had to be there.

### Epistemology of Bitcoin (some high level conclusions)

Why does it feel like explaining Bitcoin is so hard? It feels like
understanding Bitcoin has a high activation energy, with an elevated  "hump" that dissuades many people from understanding it.

Sorta like an endothermic reaction in chemistry, where there's typically an energy hump that needs to be overcome before the reaction can proceed.

![Activation energy](assets/endothermic-reaction.png)

The other thing about explaining Bitcoin is that it's a broad subject with orthogonal facets.  Explaining Bitcoin involves explaining things
that are ***related***, but ***not correlated or interdependant***.  This makes it hard to know where to start.  One finds oneself having to go back
to the beginning to introduce a new primitive concept, then moving forward with the combined abstractions, again and again.

**Explaining Bitcoin sometimes feels like a Tarantino movie**, where the story is told in a non-linear fashion, and you have to go back to the beginning to understand.

| ![](assets/pulp-fiction.jpg) |  ![](assets/kill-bill.jpg)    |
| ---- | ---- |

#### Analyzing Bitcoin subject matter

Here we try to picture and resolve why Bitcoin is so hard to explain.  We start by picking 21 facets to be explained. We could have picked 40 facets, but 
21 is ample.

If we list Bitcoin's salient subjects, and cross-reference among them for prerequisite relationships, we get a table that looks like this.

![Base concepts and their prereqisite relationships](assets/base-concepts-related.png)

**All matrices can be represented as a graph network**. Here's the graph network of these prerequisite relationships. What a mess! Where to start 
to explain Bitcoin in a coherent way?

![Base concepts and their prereqisite relationships](assets/base-concepts-graph-1.png)

Let's use a **layered graph layout** to visualize the subject prerequisite relationships. This is a little better, but it's still a mess.

![Layered format for the network graph](assets/base-concepts-layered.png)

We can **analyze the network graph for cliques**. This is interesting because
it shows how some concepts are more tightly related.  This seems to be is a promising starting point for segmenting the subject matter.

![Cliques in the network graph](assets/base-concepts-cliques.png)

What if we score subjects for their prerequisite value, their complexity (the number of prerequisites), and subtract the complexity score 
from the prerequisite value?  

In other words, the strategy is to start with the subjects that have the highest prerequisite value, and the lowest complexity.

This gives us a pretty nice roadmap! 

|   prerequisite value (P)  | complexity (C)  | P - C  |
| ---- | ---- | ---- |
| ![](assets/scores-prerequisites.png) | ![](assets/scores-complexities.png) | ![](assets/scores-prerequisites-complexities.png) |

### BTC, satoshis, and unit bias

Bitcoin values are expressed in satoshis. 1 BTC is 100,000,000 satoshis. This is why we see at most 8 decimals in Bitcoin values.

![8 decimals](assets/eight-decimals.png)

Note that, when we express a value denominated in BTC, we typically get a decimal value. Fun fact: this is the ONLY place in the Bitcoin universe 
where we see a real number, or a decimal of any sort. Bitcoin world is all about integer values only.

![8 decimals](assets/real-number.png)

You may have heard something to the effect that ***"Bitcoin is at the leading edge of mathematics, cryptography, and computer science"***.  This is a little bit of an overstatement.  

For example, **here are some math symbols you won't see in Bitcoin**:

```
≈   𝝅   ℯ   i   √   ∂x/∂t   ∫   Σ   ∏   μ   σ   n!   ε   ∞   ÷
```

In fact, you **won't find any vectors** and **no matrices** either. There are **no angles**, there is no **trigonometry**. There are **no imaginary numbers**.  There are **no negative numbers** either. There are **no fractions**.  There are **no decimals** and, therefore, **no irrational** numbers.  
Bitcoin's math is actually accessible to anyone who has completed grade 8 mathematics.

As for cryptography, **nothing is encrypled** in Bitcoin, so there's **nothing to decrypt** either. The cryptography primitives used by the Bitcoin network is 
all about hashing and digital signatures, which widely accessible subjects, and certainly not at all "at the leading edge of cryptography."
### Hashing, blocks, proof of work, and mining

We esplain the following concepts using [Anders Brownworth's blockchain demo](https://github.com/anders94/blockchain-demo) running locally.

* hashing 
* blocks and blockchains
* proof of work 
* mining

![Anders Brownworth's blockchain demo](assets/Anders-Brownworth-blockchain-demo.png)

### How much mining is going on presently?

According to [Clark Moody's Bitcoin Dashboard](https://bitcoin.clarkmoody.com/dashboard/), on October 8, 2023, there is 422 exahashes per second (EH/s) of 
mining activity on the Bitcoin network. 

Which means, miners are presently 422 * 10^18 hashes per second.  

![](assets/mining-intensity.png)
![](assets/si-prefixes.png)
### Bitcoin's heartbeat: Block time, mining difficulty, and mining difficulty adjustments

### Halving and issuance

## Resources

These are links to things I referenced during the presentation.

- [The Animated Elliptic Curve](https://curves.xargs.org/)

- [Anders Brownworth's blockchain demo](https://github.com/anders94/blockchain-demo)

- [Clark Moody Bitcoin Dashboard](https://bitcoin.clarkmoody.com/dashboard/)

