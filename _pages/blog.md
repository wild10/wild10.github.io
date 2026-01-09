---
layout: page
title: blog
permalink: /blog/
---

# [Data Structures & Algorithms with Python](https://www.blog.com) 
---

 (Not beginer tutorial)

## Introduction and why python?.

here I will write about my journey learning DSA using python. But before I have to mention that this is not a complete guide to DSA, instead it is my personal notes and experience learning DSA using python. I will be using python 3.x and  may some c++/c programming language just to compare the performance and as an intention to choose the best langauge for implementing the right and easy way to solve the problem. finally i want to say that althought there is many programming languages like java, c# that personally learnt in the past i think for my as AI engineer python is the best choice(so just a personal opinion), said that let's start.

### What is DSA?

well while everybody that start learning programming will learn about the basic data structures and algorithms, but DSA is a bit different. I am pretty sure you will find a lot of resources online about DSA, so i will not try to explain it again, instead i will jump in to the programs and explain why we need at first to learn DSA. with simple examples.

> Notes: you can find a pleanty explanation in books as well as online: i recommend you follow : [Cracking the coding interview](https://dn720001.ca.archive.org/0/items/4-programming-interviews-exposed-4th-edition/Cracking-the-Coding-Interview-6th-Edition-189-Programming-Questions-and-Solutions.pdf), [grokking algorithms 2nd Edition](https://www.amazon.com/Grokking-Algorithms-Second-Aditya-Bhargava/dp/1633438538) and you can find a lot of resources online, for python programming as a beginner i recommend you follow [geeksforgeeks](https://www.geeksforgeeks.org/)

### here is where i started:

If you are still here reading i will explain you how I started myself figure out why this is important in 2026, this. as an Machine Learning + AI Engineer that previously worked in a company building, fine-tunning, and most importante who know the core of the modern LLMs. I saw many people that are using LLMs for generate programs without noting the real good or not of the code generated. and this is a big problem, because if you are not programmer or don't know about programming when something happen you will really in a neightmare, there are many reasons that some guys wrote [Don´t be a vibe coder](https://medium.com/data-science-in-your-pocket/dont-be-a-vibe-coder-30fa7c525971), and as an engineer we want something not just work, we can something scalable, with good engineering techniques, and maintable. this is where DSA comes in, okay now less words and start coding.

### the first program [ fibonacci Numbers]

everybody know the fibonacci sequence: the story start about famous rabits that were left in a village to reproduce and after a certain period of time we want to know how many rabits we have. The really true is that Fibonacci invented this scenario and used it to explain his famous problem in his math book in the 12th century. yeah this is old math problem.

---

- here is the thing:
1° month  --> 1 couple of  rabits
2° month --> 1 couples of  rabits
3° month --> 2 couples of rabirts
4° month --> 3 couples of rabirts
5° month --> 5 couples of rabirts
6° month --> 8 couples of rabirts
7° month --> 13 couples of rabirts ... 

okay if you see the pattern we can write a program to calculate the number of rabits in the n° month so the formula is:

$$
fib(n) = fib(n-1) + fib(n-2)
$$ 

This is already know for us. so i can write simple recursive function in python to calculate the number of rabits in the n° month.

```python 
def fib(n):
    if n <= 1:
        return n    
    return fib(n-1) + fib(n-2)

if __name__ == "__main__":
    N = 5
    result = fib(N)
    print(result)
```
**is this good right?***, the simple answer is yes, but this is not the best way to write this program, this has some limitations: 
- 1. it is not efficient, it has a time complexity of O(2^n) and a space complexity of O(n).
- 2. it is not scalable, it will take a lot of time to calculate  fib(10000000).

Okay , so we can write another option, right yes there is another iterative option, as you may thing you can write this code like:

```python
def fib(n):
    if n <= 1:
        return n    
    a, b = 0, 1
    for i in range(2, n+1):
        a, b = b, a + b
    return b

if __name__ == "__main__":
    N = 5
    result = fib(N)
    print(result)
```
may you are thinking of this is better, yes now the big o is linear O(n) and if you care about the space complexity it becomes constant O(1). but we still can improve this algorithm, we can use dynamic programming to store the results of the previous calculations and avoid redundant calculations. why? because we are calculating the same values multiple times in the recursive function, so if we store the results of the previous and access directly it becomes faster.

```python
def fib(n):
    if n <= 1:
        return n    
    dp = [0] * (n+1)
    dp[1] = 1
    for i in range(2, n+1):
        dp[i] = dp[i-1] + dp[i-2]
    return dp[n]

if __name__ == "__main__":
    N = 5
    result = fib(N)
    print(result)
```

and now the big of the dinamic programming of fib(n) is O(n) and the space complexity is O(n).


so, what is the best algorithm of fib(n)?, the answer is everyone has its own advantages, even though the recursive function is not the faster it is clear and easy to understand, the iterative function is faster but it is not clear and easy, the dinamic programming is faster but the algorithm becomes complex. when we use which one depends on the problem we are trying to solve.  some algorithms like recursive function were highly used in trees and graphs, where the complexity is the main issue. so we need an algorithm that is easy to understand and not caring much about the time. Iterative algorithn on the other hand use to be difficult and brute force way to solve a problem, but it is still good in some cases as here(the best) , and first Not all the Dinamic programming algorithms are the best. in this example we can se that the DP implemention is slower.