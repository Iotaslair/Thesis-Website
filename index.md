---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: An Automated approach to Software Engineering Team Creation
layout: default
---

# What's this website for?

This website is a rough estimate for what a manager will see when utilizing the software set out in the Baccalaureate thesis titled "An Automated approach to Software Engineering Team Creation" created by [William Pembleton](https://github.com/Iotaslair). If you want to see the source code for the algorithm made in the thesis [click here](https://github.com/Iotaslair/Thesis-Project). If you want to read the paper you can [read it here]().

# What does the thesis cover?
The thesis covers explores the idea of using the [Five Factor Model](https://en.wikipedia.org/wiki/Big_Five_personality_traits) and the [Multidimensional Work Ethic Profile (MWEP)](https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.632.514&rep=rep1&type=pdf) to create an algorithm to group people together into compatible Software Engineering teams.

# What is the Five Factor and MWEP models?
So let's split this up into two section, one for each model.

## Five Factor model
This model comes from the field of Personality Psychology. There are five traits that the Five Factor model uses listed below. These traits are a continuum and you can be high in low in each of these traits.

![Five Factor model image](/ffm.png)

You may have run into other personality models during your life time such as the [Myers–Briggs Type Indicator (MBTI)](https://en.wikipedia.org/wiki/Myers%E2%80%93Briggs_Type_Indicator) or the [DISC model](https://en.wikipedia.org/wiki/DISC_assessment) however for one reason or another these models no longer have Personality Psychology's stamp of approval.

Fun fact: The Five Factor model also has a few other names like the OCEAN model or the CANOE model

## MWEP Model
The MWEP model came from [a paper by Miller, Woehr and Hudspeth](https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.632.514&rep=rep1&type=pdf). It's been cited over 550 times according to Google Scholar.
The model argues that the cultural idea of Work Ethic doesn't really make sense. Instead they argue that Work Ethic should be split up into seven different dimensions (pictured below).

![MWEP Model questions](/work ethic.png)

# So how does your algorithm do something so subjective like organizing people?
With a lot of research is the answer. The algorithm's creator read through the literature about how to make teams and used information from the paper, interviews with real Software Engineers and their best judgement to create a useful tool.

# How does the algorithm work?
The algorithm works via two methods. The first thing that it does is that it brute forces every combination of people into teams. Then it goes and scores each team. The method averages the team's traits and compares it to the "Theoretical best team" (that a manager can change). The closer the team is to the "best team" the higher their score. The other method is using a variety of tests. For instance one the tests tests that the number and introverts vs extroverts is in a certain range of values.
[To see the team recommended by the algorithm click here](./team)

# Is this going to replace hiring manager's jobs?
Short answer: No

Longer answer: No, because this algorithm can serve as gut check for if a team can really work. It does a ton of calculations that a human wouldn't want to do to provide a recommendation. That's all it really is, a recommendation. If a manager has other ideas for how to create a team or disagrees with the team recommended, then they can either disregard it or change how the algorithm scores teams to their liking. If you want to see what the setting page looks like [click here](./settings).

# What's the use case for something like this?
There's a few use cases for a tool like this.

* Making a new team
* A person just left and you're looking to hire the best person for this specific team
	* In this case a the rest of the team can be 'locked in' meaning the algorithm will search through all the other applicants and choose the appplicant that is the most compatible
* Team Shuffling/Department Shuffling
	* If a few teams are changing who is on them or a whole engineering department is being changed (such as an acquisition)

# Links to other pages
[Click here to see the team that the website recommends](./team)

[Click here to see settings for the recommendations](./settings)