---
layout: post
title: Batch effects in single cell RNA sequencing 
image: /img/scBatch1/toyClusters.png
draft: false
subtitle: Part 2 - Dealing with batch effects
---

In my [previous post](..) I discussed how the diagnosis of a batch effect in single cell data is almost always a subjective biological decision.  If you haven't read it, I suggest you do before proceeding.  But suppose you have understood the caveats and decided that you have a batch difference that really must be removed to make sense of your data.  How to proceed?

This is a fast moving area and my own set of "best practices" for processing single cell data are constantly changing.  With that caveat, this should give you some idea for how I think about processing single cell data with batch effects.

# Where do batch effects come from?

I sometimes see batch effects described like they're some bacterial infection the data picked up going about its busy life.  Our data has batch effects, no point worrying about where they got it, just give it the antibiotics and get rid of it.

Of course, when we talk about batch effects, what we really mean are systematic differences between different parts of the experiment that we want to remove.  Variability we didn't want and obscures what we care about.  Sometimes these are biological differences we don't care about, but mostly the presumption is that the differences are driven by technical effects.  Most often, this will be driven by a multitude of big and small differences, each contributing a part of the overall technical variability.

Perhaps we used different batches of reagents for different samples.  Or used kits with different chemistries.  Or entirely different single cell sequencing platforms.  Or the sample had to be kept on ice over night one time.  Or we varied the tissue dissociation protocol.  Or different samples were run on different sequencing runs.  Each of these changes may introduce different changes to the resulting data.

While some of these differences will result in transcriptomic changes that are hard or even impossible to predict and reverse, others are not.  So the first thing to do with a data set hampered by batch effects is to remove those effects you know are technical and not of interest.

# Remove what you know shouldn't be there.

Usually when I write these posts I try and use data that is freely available so you can reproduce what I've done if you really want to.  Unfortunately, some of the technical effects depend on specifics of the data that I only have readily available for my data.

What are some technical drivers of batch differences in single cell data that can be understood and removed?

## Index swapping

## Doublets

## Contamination

## 
This 
This usually https://www.nature.com/articles/s41467-018-05083-x


