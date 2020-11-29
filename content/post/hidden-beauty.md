---
title: "The Hidden Beauty of (Mathematical) Irrationality"
date: 2019-05-23T16:15:04-03:00
hero: /images/sunflower.jpg
excerpt: "The Golden Ratio, Fibonacci, and how sunflowers carry the universe in them."
description: "This is a meta description"
---
The words which you are reading now have no objective truth behind them. How could they? We invented them. Every single language on Earth is a human invention, designed to facilitate communication and ultimately enable us to work together cohesively. It is in fact the greatest human invention, since it is the one which all others are built upon.

However, despite its unparalleled utility, languages are only useful for communicating with other humans. If we wanted to communicate with the universe, how could we speak? One of the answers is through mathematics – the studies of patterns, truth, and reality itself.

My goal with this post is to illustrate an incredibly interesting way in which nature communicates with us – through the Fibonacci Numbers & the Golden Ratio – and how our understanding of mathematics has enabled us to understand what nature is trying to say.

Disclaimer: I am by no means a mathematician or expert on this topic, I am just trying to share something I am fascinated by. If you see anything wrong, please feel free to correct me.

### What are the Fibonacci Numbers?

The Fibonacci numbers are a sequence of numbers. The law governing this sequence is this:

Fn = Fn-1 + Fn-2

This means that the next number in the sequence is equal to the sum of the two previous numbers. For instance, the sequence

F = {1, 1} will become

F = {1, 1, 2}, since 2 is equal to 1 + 1,

then F = {1, 1, 2, 3}, since 3 is equal to 2 + 1,

then F = {1, 1, 2, 3, 5, 8, 13} and so on, indefinitely if you wish.

These numbers appeared in the Western world in the 13th century, when a man named Leonardo of Pisa introduced them in his book *Liber Abaci*. However, it is believed that these numbers were known as early as 200 BC.

The scope of the mathematical functionality of this sequence is beyond the scale of this post, but there are very interesting properties about these numbers, and people have been fascinated by them for a long time.

However, the one of the properties which has perhaps fascinated people the most is this:

**The division of adjacent Fibonacci Numbers gets infinitely closer to the Golden Ratio, (also illustrated as the symbol Ф, “Phi”)  or 0.618033…**

### One of the relationships between Fibonacci and Ф

Let us list the first ten Fibonacci Numbers:

F = {1, 1, 2, 3, 5, 8, 13, 21, 34, 55}

Now lets divide the adjacent numbers:

( 1 / 2 ) = 1.5

( 2 / 3 ) = 0.66

( 3 / 5 ) = 0.6

( 5 / 8 ) = 0.625

…

( 34 / 55 ) = 0.61818181818

(PS: People also refer to the Golden Ratio as 1.618033... instead of 0.618033. These numbers are interchangeable.)

As we can see, these numbers when divided get closer and closer to 0.618033.

What is the meaning of this number? Again, the beauty of this seemingly unimportant number is beyond the scope of this post, but I will focus on one point – Botany.

Forget everything you know for a minute and imagine you are a sunflower. Being a sunflower is not easy. It means you need to think deeply about how you are going to space out your florets (seeds) so that they can all receive sunlight, while growing as many seeds as you can. To that extent, an immediate thought will occur to you – **what is the optimal way to allocate seeds?**

Before thinking about the optimal solution, lets consider what you need to do. A good starting point would be to grow one seed right ahead of you, turn around a little, plant another, turn a little more, plant another, and so forth. This way, you are planting seeds all around you, right?

Yes and no. The crucial point is this: **the amount of a rotation between planting each seed**. If you planted a seed, did a full turn, planted another, did a full turn, and planted another, you’d have a straight line until you couldn’t plant anymore. That is poor design, because you want to maximize the space used around you, and by turning that much you left a lot of space unused.

I have a made a small [visualization tool](https://c.simmer.io/static/unityFrame/index.html?url=https%3A%2F%2Fsimmercdn.com%2Funity%2FcxoIdydXsyMr1reTpiqUsm2YJcI3%2Fcontent%2F10062dd3-e3f5-af79-0320-aeb1e2ad48c8&imagePath=screens/0.png%22%20style=%22width:650px;height:650px;border:0) to help us pretend you are a sunflower. Try playing around with it and inputting different rotation amounts. Here are a few fun numbers to try: 0.10, 0.33, 0.501, or anything you want!

NOTE: I built this using Unity and WebGL, and it will not work properly if you are on a mobile phone. Here is the source [code](https://github.com/Capm96/Visualizations/blob/master/Golden%20Ratio/Assets/Scripts/Flower.cs) if you are interested.

### Figuring out the optimal rotation amount

Well then, how do we figure out the optimal rotation amount? The truth is, there is a straight forward way of doing it. We can already eliminate every rotation amount that represents a rational number.

Why? Because if you rotate by any amount which is rational, eventually you’d find yourself in a position with lines of seeds and empty space between them. To illustrate, try putting in rational rotation amounts, i.e. 0.25, 0.50, 0.75, 1, etc.

But what about irrational numbers? The fascinating thing about irrational rotation amounts is that there is a positive relationship between how sparse the distribution is, and how irrational the number is. Here are three fun irrational numbers for you to try: π (3.1415), √2 (1.414), and Ф (0.610833).

Notice that even though π is an irrational number, its configuration doesn’t seem very optimal. It gets better with √2, but it is the best with Ф.

**Therefore, it seems that the optimal amount of a turn we must do should be the most irrational of all numbers. And that is precisely Ф.**

### Why the Golden Ratio is the most irrational of all numbers

Before we talk about Ф, let’s use π as an example.

As you may know, π is infinite as far as we can tell. We can approximate it, and we can get a very close approximation, but it is never “enough”. This is usually the way irrational numbers go -- they cannot be expressed as fractions, and go on for ever and ever.

In any case, this means that we can define π for our purposes as something like: 3.14159265359

However, I lied. We can also illustrate π as a fraction! But it must be a special kind of fraction.

What we need is a “Continued Fraction". This is a fraction that goes on forever and ever, in the same way that π does. Instead of displaying π as decimal, we are displaying it as a fraction -- and neither of them ever terminate.

Here is what the beginning of π's continued fraction looks like:

![Image](/images/blog/flower/fraction1.jpg)

If you try to truncate, i.e. cut short, the continued fraction at some point, you will get an approximation of π. This approximation's accuracy depends on where you truncate the continued fraction.

For instance, imagine we truncate the continued fraction above right after the "+" sign next to the 3. We would truncate it at the very beginning, and we would end up with 3 -- which is close to π, but we can do better.

If we truncate it after the 1/7, we would get 3 + (1/7) = 3.14... this is already a better approximation, which means truncating the fraction here would yield a closer approximation.

The question is then, at which point could we truncate this continued fraction to get a very good approximation? And the answer is at the point which that particular fraction does not add too much accuracy -- in other words, look for a fraction there with a very large denominator.

The 1/292 suits our needs. This means that if we truncate the continued fraction at that point, the following fractions will not add too much accuracy, because this fraction (1/292) was already extremely accurate -- meaning that everything that preceded this was already a good approximation to π.

Therefore, it seems we can approximate irrational numbers by truncating them at specific points in their continued fractions, and the fraction at which we truncate them helps us determine the degree of accuracy of the irrational number at that point. As we saw, for π, we don't need to go very far to get a really good approximation -- when the continued fraction reaches the 1/292 fraction, π is already well-approximated.

Now lets take a look at the continued fraction for Ф.

![Image](/images/blog/flower/fraction2.jpg)

Do you notice anything different from π’s?

The fractions are all the same! There is no “best” point to truncate the continued fraction at, because all of the fractions have exactly the same denominator. This means that unlike π, which we could approximate early on, Ф has no early approximation -- every fraction adds as much accuracy as the previous.

Because of this, Ф is the most irrational of all numbers.

Also, if you go back to the visualization and count the number of spirals in the 0.618033 rotation, you will get a Fibonacci number. In fact, these Fibonacci Numbers are present in a plethora of configurations within nature. So is Ф.

This post illustrated just one way in which Nature, the Fibonacci Numbers, and the Golden Ratio are interlinked. There are so many other incredible examples which I have not covered in this post, but which I encourage you to search.

### Closing thoughts

I find it remarkable that such a seemingly uneventful number is so omnipresent in our world. It is not a coincidence that sunflowers have a Golden Ratio configuration -- it is simply the best way to do it. How could it not be? As we saw, for one very specific example, it is the optimal solution to a problem.

The beauty of all of this is that we had absolutely nothing to do with it -- it was nature herself who adjusted the properties of the universe to maximize her utility. None of this was random. There are a set of rules governing our reality and everything must abide it, from seeds to galaxies.

As I mentioned earlier, languages are human constructs, whereas mathematics is a built-in feature of the universe itself. There is no such thing as inventing mathematics, there is only discovery, because all of its inventions are already done -- it is only up to us to figure it out now, one sunflower at a time.

### Sources:

[The Golden Ratio (why it is so irrational)]( https://www.youtube.com/watch?v=sj8Sg8qnjOg)

[Algorithmic Botany]( http://algorithmicbotany.org/papers/abop/abop-ch4.pdf)

[What is the Golden Ratio?]( https://www.livescience.com/37704-phi-golden-ratio.html)

[Doodling in Math]( https://www.youtube.com/watch?v=ahXIMUkSXX0)

[The Mathematical Magic of the Fibonacci Numbers](http://www.maths.surrey.ac.uk/hosted-sites/R.Knott/Fibonacci/fibmaths.html)

[Golden Ratio Proof](http://jwilson.coe.uga.edu/EMT668/EMAT6680.2000/Burrell/Assignment12/goldenratioproof.html)

[Other places where Ф is present](https://io9.gizmodo.com/15-uncanny-examples-of-the-golden-ratio-in-nature-5985588)

[Where I got the picture for this post](https://www.google.com/search?q=sunflowers&client=firefox-b-d&source=lnms&tbm=isch&sa=X&ved=0ahUKEwih04zRiMTiAhUMErkGHRLeAl4Q_AUIDigB&biw=1536&bih=767#imgrc=HPHoWJcTU7QxDM:)