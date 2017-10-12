---
layout: page
subheadline: Python
title:  "Useful Python Functions"
teaser: "Python supplies a variety of useful functions that beginners coming from other languages may not know about. Here are a few of them."
meta_teaser: "Python supplies a variety of useful functions that beginners coming from other languages may not know about. Here are a few of them."
breadcrumb: true
categories:
    - python
tags:
    - python
    - programming
    - tips
    - beginner
image:
    title: blog/python-logo.png
author: SZanlongo
---
## zip
[`zip`](https://docs.python.org/3.5/library/functions.html#zip) provides a way of iterating over multiple lists at the same time. This moves left-to-right over the lists until the shortest one is exhausted.

As an example:

    >>> a = [1, 2, 3]
    >>> b = ['a', 'b', 'c']
    >>> c = zip(a, b)

Keep in mind that `zip` returns an iterator, so doing something like `print(c)` will only return the object: `<zip object at 0x000002730FA94AC8>`. This is because the return values are generated as needed (good for reducing memory usage!). If we want to see the output all at once, we'll have to ask for a list:

    >>> print(list(c))
    [(1, 'a'), (2, 'b'), (3, 'c')]

## List Comprehension
[List comprehension](https://docs.python.org/3/tutorial/datastructures.html#list-comprehensions) takes in source values, and generates a list of result values, allowing you to apply an operation on each value. It is basically another way of writing a for-loop, but is useful when doing small operations.

A basic example of list comprehension would be:

    >>> a = [1, 2, 3]
    >>> b = [x * 2 for x in a]
    [2, 4, 6]

List `b` will be comprised of the elements of `a`, where each element has been multiplied by 2.
Keep in mind that the input need not be a list, we could also use a generator such as:

    >>> b = [x * 2 for x in range(1, 4)]
    [2, 4, 6]

which accomplishes the same as the previous example, but using the `range` generator. List comprehension can also be nested. This is equivalent to nested for-loops, and is often used when handling multidimensional arrays:

    >>> a = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
    >>> b = [[x * 2 for x in row] for row in a]
    [[2, 4, 6], [8, 10, 12], [14, 16, 18]]

This also ties in nicely with our next built-in function, `product`.

## Product
[`product`](https://docs.python.org/3/library/itertools.html#itertools.product) is similar to nested for-loops or nested list comprehension, providing the Cartesian product of the input iterables in lexicographic order. This makes it especially useful when iterating over all the elements of a matrix.

For example, let's say we need to go over all the `x, y` - pairs, so that `0 < x < 10` and `0 < y < 10`. We can accomplish this as follows:

    >>> from itertools import product
    >>> for x, y in product(range(1, 10), range(1, 10)):
    ...    print(x, y)
    1 1
    1 2
    1 3
    ...
    9 7
    9 8
    9 9

Notice how the `y` - value loops from `1` to `9` before `x` updates, this is the lexicographic ordering at work. The equivalent nest for-loop would be:

    >>> for x in range(1, 10):
    ...     for y in range(1, 10):
    ...         print(x, y)

## Other Posts
{: .t60 }
{% include list-posts tag='post format' %}
