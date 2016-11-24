extends: default.liquid

title: Wikilinks
github-link: https://www.github.com/stensonowen/wikilinks
demo-link: http://www.wikilinks.xyz:16687/
type: project
subtitle: (this is a subtitle 1)
description: Represent the internal links between Wikipedia pages with a hash table and perform a breadth-first search between any two articles. Link data is parsed from monthly (-ish) Wikipedia dumps and stored so it can be read from a file every time the program runs. We then hash each article's title to determine its index in the hash table; the rest of the program reasons using this index, as it is much more efficient to store and compare 32-bit integers rather than arbitrarily long strings. Nonetheless, this has some scalability issues; despite its memory being almost entirely vectors of integers, it still requires about 10GB for the English Wikipedia dump, and despite being multithreaded it still requires several minutes to populate the hash table. These benchmarks are much better than they used to be, though.
date: 13 January 2016 21:00:30 -0500
---

# Wikilinks

A bunch of stuff about wikilinks
