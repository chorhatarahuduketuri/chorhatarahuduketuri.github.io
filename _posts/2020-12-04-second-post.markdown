---
layout: post
title:  "Advent of Code"
date:   202012-04 17:34:26 +0100
categories: admin update
---

# Things I am doing (and have done)

##### The 'oh yea I should actually write something' post

### Advent of Code

So I'm doing the [Advent of Code][aoc] game this year, and I'm playing in Python, and today wrote my first dict of lambda functions, because why wouldn't I? I shall now display it to you:

{% highlight python %}
valid_fields = {
    'byr': lambda x: 1920 <= int(x) <= 2002,  # Birth Year
    'iyr': lambda x: 2010 <= int(x) <= 2020,  # Issue Year
    'eyr': lambda x: 2020 <= int(x) <= 2030,  # Expiration Year
    'hgt': lambda x: check_height(x),  # Height
    'hcl': lambda x: re_hcl.match(x),  # Hair Color
    'ecl': lambda x: re_ecl.match(x),  # Eye Color
    'pid': lambda x: re_pid.match(x),  # Passport ID
}
{% endhighlight %}

### Why

Yes, why would I perform work no one will ever see for magic internet points, because no on ever does that. But mostly so that I actually get to write code most days, mostly at the same time, and get into the habit of making something every day. 

### What else

I could also write here every day, which would also be creating something, but then I don't really feel the need to say something every day (not that I _can't_ waffle on as much as the next human.) I should probably get round to writing about the bookcase construction (with timelapses of me and my electric screwdriver) and the bicycle. It would probably encourage me to do more construction, which would be a good thing given how long I've already (two months!) been stuck in a flat with no windows. 

Also, it appears rather evident that I could do with more practice writing. 

OK yea I might as well keep this updated with how the Advent of Code is going. 

[aoc]: https://adventofcode.com/2020
