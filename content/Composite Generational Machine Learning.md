# But how does regular Generational Machine learning work?

## First, an explanation about regular generational machine learning.
Generational Machine learning as the name implies, is a method through which you have individual generations of whatever population you are training. After a population is finished, you pick the best performing couple and then reproduce the entire population using slight variations on that model.

## What are the disadvantages?
Generally you will find that over the course of training a specific model, the value hereby referred to as the learning modifier, is a value that modifies how much change each individual generation goes through. In standard Generational Machine Learning you will find that this is a single global value that decreases over time, to allow for large learning steps in the beginning of training, and small fine tuning steps in the later stages. This leads to a large problem, the later stages can't learn anything new. 

# The Composite Solution

## What is it?
My idea is to instead of using a global learning modifier value, have several different values that apply to the population. Let's say we have 85% of the population that are "Fine Tuning" (FTMs, another 10% that are changing moderately (MCMs) and another 5% that are the "Large Change Models" (LCMs).
## An Example
Let's say we're training a [machine learning model to drive cars in a racing game.](https://www.youtube.com/watch?v=Dw3BZ6O_8LY) The model has learned pretty well, and is finishing most of the time, but in it's late stages all it can really do is drive the same way but better. With this new method you have a subpopulation of each generation driving a moderately or drastically different way. Most of the time they will fail, but what if they stumble upon something big?

## But how will the LCMs keep up?
Now, you might be thinking something along the lines of "But how will the LCMs keep up with the FTMs? Sure they might discover something new, but without practice they will be slower anyway!" This is where something I will call "Generational Persistence" will kick in. Effectively guaranteeing that some practice will be had with these drastic changes by forcing these MCMs and LCMs to persist for several generations even if they don't do well. Then, if they still fail after further training we can safely remove them.

# Conclusion (TLDR)
Composite Generational Machine Learning will allow for large changes to the model even late in its training by having a subset of each generation's population do more than just have changes meant for fine tuning.


### Is it my idea? I have no damn clue!
I am unsure if this is actually my original idea, maybe someone else has thought of or done this before, but as far as I am aware it is not in mainstream use as I have never seen it used anywhere.