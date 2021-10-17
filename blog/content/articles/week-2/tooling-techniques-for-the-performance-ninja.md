---
title: ⚙️ Tooling techniques for the performance ninja
tags: [techniques, performance, week-2]
layout: post
url: articles/tooling-techniques-for-the-performance-ninja
author: Eduardo Flores
publishdate: 2021-10-17T13:33:00.000Z
summary: The secret to creating a high-performance website lies in the ability to gather insight about issues, and quickly iterate on solutions.
---

# 3 steps to the performance tuning loop

### Get data

Get information on why your website is slow.

### Gather insight

Turn that data into improvment ideas.

### Take action

Improve your website based on the insights you collected.

# Three pilars of web performance

## Network

How fast your website is responding to requests and how that affects load time. The most important part of this process is the critical path.

The critical path is the resolution of the dependencies of your assets.

### How to solve this?

We need to optimize the critical path, reduce the number of dependencies in it. The more request you're making, the more overhead you're adding to your time.
Next, we need to reduce the size of our webpage.

- Reduce number of requests.
- Reduce number of bytes needed. (CSS, JS, images)

## Rendering

How fast your website is rendering content and how can you modify your code to make it faster.

### How to solve this?

Reduce number of paints, don't change the DOM if you don't absolutely have to, this will consume more resources.

Of course, this is not a problem with modern frameworks like React, which is a library that does all the DOM manipulation for you and saves up resources, among other things.

## Compute

How fast your website is performing computations.

### How to solve this?

Reduce JavaScript execution time.
