---
layout: post
title: "Do I have to learn how to analyse algorithms?"
description: "Why it is important to know how to analyze algorithms?"
category: Algorithms 
tags: [algorithms, complexity, master]
---
{% include JB/setup %}

<p align="justify">
This year I started a master course in computer science at PUC-RIO.
In my course one of the mandatory subjects is "Project and Analysis of Algorithms". 
This subject is very difficult for me, but it is very important too.
Therefore, I decided to share what I am learning about it. 
Firstly, I will try to give a brief introduction about algorithms. 
Secondly, I will enumerate some reasons to learn how to analyse algorithms.
And, to summarize, I will give a classical example of algorithm analysis.
</p>

## What is an algorithm? ##

<p align="justify">
As you can see in several books and websites, an algorithm is a procedure to do something in a finite number of steps.
We use algorithms all the time, for example when we are driving, cooking, brushing teeth and so on.
In computer science the tasks performed by software systems are specified by algorithms. 
I won't spend much time in this topic. Its purpose is just to contextualize and refresh your memory. So let's go to the point.
</p>

## What is algorithm complexity and why analyse it? ##

<p align="justify">
It is possible to analyse both correctness and complexity of an algorithm. 
As you can immagine, we analyse the correctness to check if the algorithm does exactly what he intends to.
It is an important subject, but, here, I will focus only in the complexity.
</p>
<p align="justify">
Analysing the complexity of an algorithm has as main goal predict the resources required by the algorithm.
Such resources can be memory, communication bandwidth or logic gates, but, in general, we measure computational time.
We analyse the running time of an algorithm based on the input size of the problem, ie,
we measure the number of "steps" executed by the algorithm given an input of size n.
</p>

## Is it necessary?

<p align="justify">
You may be wondering why not just execute the algorithms to see which runs faster.
The answer is that analysing the complexity before implementing is, in general, faster and easier than 
implement and test several algorithms.
Some solutions can be discarded without even writing the pseudo-code.
Furthermore, when you have enough practice you will be able to recognize patterns that characterize more complex algorithms,
and so you can apply techniques to break such complexities.
Let's do a classical example to see what we take into consideration when analyzing algorithms.
</p>

## Example

If you have to sort a list of integer, how would you do that?

<p align="justify">
Well, a simple solution would be the following: repeatedly step through the list,
comparing each pair of adjacent numbers swapping those that are in the wrong order.
Such algorithm is known as "Bubble Sort" and you can find several implementations on the internet.
The worst case of "Bubble Sort" is when the list is sorted in descending order.
For instance, in the following list we have 4 elements:
</p>

### | 4 | 3 | 2 | 1 |

Using the "Bubble Sort" algorithm, we would do the following comparisons and swaps:

### | **4** | 3 | 2 | 1 | -> | 3 | **4** | 2 | 1 | -> | 3 | 2 | **4** | 1 | -> | 3 | 2 | 1 | **4** |

### | **3** | 2 | 1 | 4 | -> | 2 | **3** | 1 | 4 | -> | 2 | 1 | **3** | 4 | 

### | **2** | 1 | 3 | 4 | -> | 1 | **2** | 3 | 4 |

### | **1** | 2 | 3 | 4 |

<p align="justify">
Considering n as the number of elements in the list, in the worst case we make n(n +1)/2 comparisons, which is equals to (n² + n)/2
To analyse algorithms it is common to use a notation called "Asymptotic Notation". 
Such notation characterizes algorithms according to their growth rates. 
Considering c as being the constant factor of the function we have c = (1/2), so
</p>

(n² + n)/2 = c * (n² + n) 

<p align="justify">
In Asymptotic Notation the constant factor is omited, thus the complexity of "Bubble Sort" in the worst case would be (n² + n).
But when n is big enough, the term of the highest order makes the remaining terms insignificant.
For this reason, the complexity of "Bubble Sort" in the worst case is n².
To analyse an algorithm asymptotically it is common to use three different notations: Big-O, Omega and Theta.
At the moment I will limit myself to say that the Big-O notation sets an upper limit for the algorithm's growth function.
Therefore, the complexity of our "Bubble Sort" algorithm is O(n²).
</p>

### Can we do Better?

Of course we can. There are several algorithms better than this one. But I will not talk about them today.
You can find a very good article about [sorting algorithms][1] at Wikipedia.

## Conclusions

<p align="justify">
In this post I tried to give a brief introduction about algorithms complexity.
In our example we had an introduction to asymptotic notation using one of the most well-known sorting algorithms.
I hope this post helps beginners in this area.
I omitted several things to keep the post as simple as possible, but I will try to address these questions in future posts.
Feedbacks are always welcome.
</p>

[1]: https://en.wikipedia.org/wiki/Sorting_algorithm
