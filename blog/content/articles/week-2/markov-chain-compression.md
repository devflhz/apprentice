---
title: 🇷🇺 Markov Chain Compression
tags: [compression, week-2]
layout: post
url: articles/markov-chain-compression
author: Eduardo Flores
publishdate: 2021-10-17T16:47:00.000Z
summary: Markov Chains Compression sits at the cutting edge of compression algorithms.
---

Markov Chains is a mathematical system that undegoes transitions from one state to another state on a state space and is generally characterized as memory-less.

The state depends only on the current state and not on the sequence of events proceding it providing that applications follow statistical models of real world processes.

It sits at the cutting edge of compression algorithms.

Markov chains allows us to identify the transitions between nodes using codes, when a transition is simple, meaning that it only has one transition, we shouldn't need more than one bit to identify it, that's where VLC or Variable Length Codes comes in. in order to make it efficient we need to use VLC to encode the transitions with the least amount of bits possible.

The probability of a transition from one state to another is determined by the number of times the current state has been encountered, each context transition manages it's own probability table, allowing it to have its own VLC set.
