---
layout: post
title: "Introduction to Algorithms Complexity"
description: "Introduction to algorithms complexity analysis"
category: Project and Analysis of Algorithms 
tags: [algorithms, complexity, master]
---
{% include JB/setup %}

<p align="justify">
This year I started my masters course in computer science at PUC-RIO.
In my course one of the mandatory subjects is "Project and Analysis of Algorithms". 
This subject is very difficult for me, but it is very important too.
Therefore I decided to share what I am learning about it. 
Firstly, I will try to give a brief introduction about algorithms. 
Secondly, I will enumerate some reasons to study algorithms complexity.
And, to summarize, I will give a basic example comparing two different algorithms that solve the same problem.
</p>

## What is an algorithm?

<p align="justify">
As you can see in several books and websites, an algorithm is a procedure to do something in a finite number of steps.
We use algorithms all the time, for example when we are driving, cooking, brushing teeth and so on.
In computer science the tasks performed by software systems are specified by algorithms. 
I won't spend much time in this topic. It's purpose is just to contextualize and refresh your memory. So let's go to the point.
</p>

## What is algorithm complexity and why analyse it?

<p align="justify">
It is possible to analyse both correctness and complexity of an algorithm. 
As you can immagine, we analyse the correctness to check if the algorithm performs exactly what he intends to do.
It is an important subject, but I won't talk about it in this post. We will focus in the complexity of algorithms.
</p>
<p align="justify">
Analysing an algorithm complexity has as main goal predict the resources required by the algorithm.
Such resources can be memory, communication bandwidth or logic gates, but, in general, we measure computational time.
We analyse the running time of an algorithm based on the input size of the problem, ie,
we measure the number of "steps" executed by the algorithm given an input of size n.
</p>
But why the hell is it necessary?
<p align="justify">
you may be wondering why not just execute the algorithms to see which runs faster.
The answer is that analysing the complexity before implementing is, in general, faster and easier than 
implement and test several algorithms.
Some solutions can be discarded without even write the pseudo-code.
Let's see a classical example to ilustrate what I am saying.
</p>

## Example

If you have to sort a list of integer, how would you do that?
<p align="justify">
Well, a simple solution would be the following: repeatedly step through the list,
comparing each pair of adjacent numbers swapping those that are in the wrong order.
Such alogrithm is known as "Bubble Sort", and you can find several implementations on the internet.
The worst case of "Bubble Sort" is when the list is sorted in descending order.
For instance, in the following list we have 4 elements:
</p>

### | 4 | 3 | 2 | 1 |

Using the bubble sort algorithm, we would do the following comparsions and swaps:

### | **4** | 3 | 2 | 1 | -> | 3 | **4** | 2 | 1 | -> | 3 | 2 | **4** | 1 | -> | 3 | 2 | 1 | **4** |
### | **3** | 2 | 1 | 4 | -> | 2 | **3** | 1 | 4 | -> | 2 | 1 | **3** | 4 | 
### | **2** | 1 | 3 | 4 | -> | 1 | **2** | 3 | 4 |
### | **1** | 2 | 3 | 4 |

Considering n as the number of elements in the list, in the worst case we make n(n +1)/2 comparsions, which is equals to (n² + n)/2
To analyse algorithms it is common to use a notation called "Asymptotic Notation". 
In such notation we consider only the highest order elements of the complexity function. 
For this reason the complexity of "Bubble Sort" is O(n²).





## Conclusions



