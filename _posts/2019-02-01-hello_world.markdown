---
layout: post
title:  "What am I doing with my life?"
date:   2019-02-01 10:21:03 +0300
categories: posts
---

When I tell people about what I'm doing with my day-to-day life people usually raise an eyebrow when I'm coupling the words trusted execution environments together.

So what are trusted execution environments? Well first its probably too long to repeat these every time, so people usually refer to them as TEEs.
TEE basically provides a secure and isolated execution region.
The automatic question is then, how are they different than the traditional paradigm where process isolation
provided by current operating systems (OSes)?
Well, the main difference lies in the trust model.
TEEs do not need to rely on the OS for this isolation property,

I like the following citation from [1]:

"Suppose you are presented with two physically identical computers. One is running a highly-certified, formally-proven, time-tested software stack, while the other is running a commodity software stack that provides similar features, but is infested with sophisticated malware.
How can you tell which computer is which? How can you decide which computer you should use to check your email, update your medical records, or access your bank account?"

It is easy to understand why TEEs can help in this context. That is if we can find a way to bootstrap trust in a certain
application, say the bank application in the above example, we can conveniently trust it with our private information, e.g., credit card details.
Theoretically, it is a great vision, but as in everything in life, the devil is in the fine details.
In the next couple of posts, I will survey the current existing TEEs, and discuss how they differ in their security guarantees and how one can bootstrap trust in applications executing with them.

In case you are interested in this, what I believe to be an exciting developing area, send me an e-mail. You can also refer
to the project page to see what I'm currently looking at. Most of them usually find their way to GitHub.

References:

[1] Bryan Parno • Jonathan M. McCune • Adrian Perrig - Bootstrapping Trust in Modern Computers
