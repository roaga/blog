---
layout: post
title: Designing Technology for Unbiased Understanding of Information
---

This is a bit of an update on the AI detective board for customer discovery, [Notitia](https://notitiaworks.com).

We've been hard at work at building the core AI system, which takes notes and clusters related items on a map, showing you big themes at a glance. Now, you can even zoom out and see the key words over each cluster. With everything staring at you in the face, it's hard to fall prey to bias and ignore what customers truly need.

While I can't tell you how it works exactly, I'll share some of the thought process of it's design and how it enables better ventures. Because building something people don't want kills startups, and bias in how you understand customers makes you build that thing they don't want.

I recommend opening up [this landing page](https://notitiaworks.com) while you read to play around with the visualization and make sense of what I'm talking about. Otherwise it's just a bunch of principles.

### Categorization without Categories
When you have lots of ideas to judge, a common exercise among UX designers and others is to group sticky notes of ideas in a box to define their category. It helps filter out info and make the important themes easy to understand. But what if something doesn't fit in? It's usually put to the side. _But what if it was the key connection between the themes?_ Then you've missed something big. **When you categorize into your buckets, you're bringing in selection bias and framing bias before you've even gone through every idea.**

So in [Notitia](https://notitiaworks.com), we don't define the buckets. We use properties of language to find a coordinate for each idea on the map--clusters only come in later to help visualize what's related, because it can get quite crowded. Because of that, you'll often note clusters overlapping. **This spectrum of meaning and mixing of different buckets is where the unique insights come from!** You are free to look at the overall themes, but then dive deeper into each and see where each detail really lies in relation to its neighbors. And if another idea from the same interview is across the map in a different cluster? We draw an animated line there to nudge you to explore that connection.

From a technical perspective, this is also great. We don't have to train separately for each industry or topic or customer segment. It's all general English, plus a few entities.

### Making Hundreds of Data Points Legible at a Glance
Data visualizations with hundreds or thousands of colored dots are great when you have axes and you don't really care what each dot means. But here, every dot is a big sticky note--we do care about each one. But that's bound to get messy, no?

- With the help of some scaling functions (after the coordinates are calculated!), the spacing smooths out a bit.
- With big, colorful sticky notes, they peek out from under each other so items aren't fully hidden.
- Knowing the topic of a cluster helps you figure out what nearby notes are about without even reading them.
- Word clouds when you zoom out give you an idea of what you're looking at before you even look at it. The mess only shows up when you're diving deep into the details, at which point 90% of it is off-screen anyway.

Overall, it's pretty easy to get an idea of the big picture when looking at everything at once, and to explore relevant details when you zoom in.

### Why Visual at All?
Why visualize anything at all? Why not just write a list with some scores, and list things together?

A picture speaks a thousand words. When you see a picture, you can process so much more information so much faster. It helps reduce the information overload that you would have with hundreds or thousands of notes to sift through. Important things jump out at you before you even realize they're important. And it makes it more pleasant to use and explore.

And as I said before, we don't want to box in your thinking--we want to help you draw new conclusions and connections. If we group a bunch of paragrpahs in a table, we're acting like it's already set in stone. We've drawn a 1 pixel barrier between any connection you want to make. [Play around with it and you'll see the benefit.](https://notitiaworks.com)


