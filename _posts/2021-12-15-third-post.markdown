---
layout: post
title:  "Advent of Code 2021"
date:   2021-12-15 19:46:46 +0100
categories: admin update
---

# Things I am doing (again)


### Advent of Code (again)

So I'm doing the [Advent of Code][aoc] game this year (again), and I'm playing in Python (again), and my stretch goal is to over-engineer it as much as possible in the form of GitHub Actions, decorators, context managers, containerisation, pytest, and anything else I can think of. 

So far, I'm rather behind, because of reasons (RSI) and bad sleep (it's amazing how hard it is to sleep in that much pain - you'd think you'd pass out from the boredom of it after a while, but no.)  

This is my favourite list comprehension so far: 

{% highlight python %}
    [
        [
            [int(number) for number in line.split()]
            for line
            in number_block.strip().split('\n')
        ]
        if ',' not in number_block else
        [int(number) for number in number_block.split(',')]
        for number_block
        in open('../puzzle_inputs/day_4.txt').read().strip().split('\n\n')
    ]
{% endhighlight %}

It is day 15 now, and it was day four when I last did anything, but I've decided that getting the stars every day on the day in the morninig is a game for people who don't have to do any chores. I'll be doing as and when I cba. 

### AWS DeepRacer

I had a rather fun time over the last two days competing in an AWS DeepRacer competition. In the end I came second out of eight people. Looksee:

![DeepRacer Results Table](/img/sanitised_race_results.png) 

And here's a video of my one-second-off winning time (passive agressive model naming included):

<video width="640" height="480" controls>
  <source src="/img/aws_deepracer_video.mp4" type="video/mp4">
</video>

Not so bad given that I got about 0.75 out of 2.0 days that everyone else got, due to really weird error messages that I had no capacity to work with (the AWS DeepRacer Console doesn't realistically give you accesss to debug error messages about Kinesis streams and mp4 videos.) 

Apparently it's traditional to keep your reward functions a secret, but I'll reveal that my reward function (and entire training strategy) is based around replicating a very well understood process - learning to drive. If I ever get to take part again, I hope there are fewer errors and I get to complete my master plan of completing the track at high speed in half the time of the second place. 

Since that's very unlikely, I'll have to stick with [Advent of Code][aoc] and other public games my employer won't try to take ownership of (since they've said they would last time I wrote something to make my life easier.) 

[aoc]: https://adventofcode.com/2021
