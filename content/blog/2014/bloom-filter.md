---
title: "Bloom Filters Made Easy"
description: "Bloom filters are easy to understand with the right explanation."
date: "2014-02-11"
url: /blog/2014/02/11/bloom-filters/
credit: "https://unsplash.com/photos/eksqjXTLpak"
image: "/media/2014/02/nathan-dumlao-454456-unsplash.jpg"
categories:
  - Databases
  - Programming
---
I mentioned Bloom Filters in my talk today at [Strata](http://strataconf.com/strata2014/public/schedule/speaker/142). Afterwards, someone
told me it was the first time he'd heard of Bloom Filters, so I thought I'd
write a little explanation of what they are, what they do, and how they work.

But then I found that [Jason Davies already wrote a great article](http://www.jasondavies.com/bloomfilter/) about
it. Play with his live demo. I was able to get a false positive through luck in
a few keystrokes: add alice, bob, and carol to the filter, then test the filter
for candiceaklda.

Why would you use a Bloom filter instead of, say...

* Searching the data for the value? Searching the data directly is too slow,
  especially if there's a lot of data.
* An index? Indexes are more efficient than searching the whole dataset, but
  still too costly. Indexes are designed to minimize the number of times some
  data needs to be fetched into memory, but in high-performance applications,
  especially over huge datasets, that's still bad. It typically represents
  random-access to disk, which is catastrophically slow and doesn't scale.


