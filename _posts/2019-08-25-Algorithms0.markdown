---
layout: post
title:  "Algorithms"
date:   2019-10-04 20:34:03 +0100
categories: blog
permalink: blog/:title
intro: "Introduction to Algorithms."
---

## Algorithm Characteristics
1. Complexity
  - space (memory)
  - time
2. Input and Output
3. Classification
  - serial/parallel
  - exact/approximate
  - deterministic/non-deterministic

## Common Algorithms
* Search: find specific data
* Sorting
* Computational: take one set of data, and calculate another
* Collection: counting specific items or filtering out data

## Euclid's Algorithms
Find the greatest common denominator of two numbers using Euclid's algorithm.

### Example:

```
gcd(20, 8) = 4
```

```python
# Find the greatest common denominator of two numbers
# using Euclid's algorithm

def gcd(a, b):
  while a % b > 0:
    r = a % b
    a = b
    b = r
  return b

import ipdb; ipdb.set_trace()

# try out the function with a few examples
print(gcd(60, 96))  # should be 12
print(gcd(20, 8))   # should be 4

```

## Measuring Algorithm Performance

### Big O Notation
Classifies performance as the input size grows
"O" indicates the **order of operation**: timescale to perform an operation
