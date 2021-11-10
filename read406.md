# Big O: Analysis of Algorithm Efficiency 

## Overview
Big O’s role in algorithm efficiency is to describe the Worst Case of efficiency an algorithm can have in performing it’s job. It specifically looks at the factors mentioned above, which we often refer to as Space and Time. In order to analyze these limiting factors, we should consider 4 Key Areas for analysis:

1. Input Size
2. Units of Measurement
3. Orders of Growth
4. Best Case, Worst Case, and Average Case

**In order to quantify the Running Time in our analysis, we will consider Three Measurements of time:**

1. The time in milliseconds from the start of a function execution until it ends.
For the purposes of Big O, we won’t be considering this measurement since different machines will have different individual run times depending on how powerful they are. Regardless, this will always be a measurement of run-time.

2. The number of operations that are executed.
Think of this as the number of lines of code that are executed from start to finish of a function.

3. The number of “Basic Operations” that are executed.
“Basic Operation” refers to the operation that is contributing the most to the total running time. This is usually the most time consuming operation within the inner most loop.


**In order to quantify Memory Space, we can consider Four Sources of Memory Usage during function run-time:**

1. The amount of space needed to hold the code for the algorithm.
Think of this as the number of bytes required to store the characters for the instructions specified in your function.

2. The amount of space needed to hold the input data.
If direct input data is not considered, we may just refer to this as Additional Memory Space since not all functions have direct input values.

3. The amount of space needed for the output data.
4. The amount of space needed to hold working space during the calculation.
Working Space can be thought of as the creation of variables and reference points as our function performs calculations. This will also include Stack Space of recursive function calls … specifically how memory usage scales relatively with the size of the input.


## Orders of Growth

We can describe overall efficiency by using the input size n and measuring the overall Units of Space and Time required for the given input size n. As the value of n grows, the Order of Growth represents the increase in Running Time or Memory Space.


![img](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/images/OrdersOfGrowth.png)


## Linked Lists 

### What is a Linked List 

A Linked List is a sequence of Nodes that are connected/linked to each other. The most defining feature of a Linked List is that each Node references the next Node in the link.

There are two types of Linked List - Singly and Doubly. We will be implementing a Singly Linked List in this implementation.

### Terminology: 

1. Linked List - A data structure that contains nodes that links/points to the next node in the list.
2. Singly - Singly refers to the number of references the node has. A Singly linked list means that there is only one reference, and the reference points to the Next node in a linked list.
3. Doubly - Doubly refers to there being two (double) references within the node. A Doubly linked list means that there is a reference to both the Next and Previous node.
4. Node - Nodes are the individual items/links that live in a linked list. Each node contains the data for each link.
5. Next - Each node contains a property called Next. This property contains the reference to the next node.
6. Head - The Head is a reference of type Node to the first node in a linked list.
7. Current - The Current is a reference of type Node to the node that is currently being looked at. When traversing, you create a new Current variable at the Head to guarantee you are starting from the beginning of the linked list.

![img](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/images/LinkedList1.PNG)

## What’s a Linked List, Anyway? 

Information is all around us.

In the world of software, the ways that we choose to organize our information is half the battle. Here’s the thing though: there are so many ways to solve a problem. And when it comes to organizing our data, there are lots of tools that could work for the job. The trick is knowing which tool is the right one to use.

Regardless of which language we start coding in, one of the first things that we encounter are data structures, which are the different ways that we can organize our data; variables, arrays, hashes, and objects are all types of data structures. But these are still just the tip of the iceberg when it comes to data structures; there are a lot more, some of which start to sound super complicated the more that you hear about them.

One of those complicated things for me has always been linked lists. I’ve known about linked lists for a few years now, but I can never quite keep them straight in my head. I only really think about them when I’m preparing for (or sometimes, in the middle of) a technical interview, and someone asks me about them. I’ll do a little research and think that I understand what they’re about, but after a few weeks, I forget them again. The whole thing is pretty inefficient, and it all stems from the fact that I know they exist, but I don’t fundamentally understand them! So, it’s time to change that and answer the question: what on earth is a linked list, anyway?

### Linear data structures

If we really want to understand the basics of linked lists, it’s important that we talk about what type of data structure they are.
One characteristic of linked lists is that they are linear data structures, which means that there is a sequence and an order to how they are constructed and traversed. We can think of a linear data structure like a game of hopscotch: in order to get to the end of the list, we have to go through all of the items in the list in order, or sequentially. Linear structures, however, are the opposite of non-linear structures. In non-linear data structures, items don’t have to be arranged in order, which means that we could traverse the data structure non-sequentially.

![img](https://miro.medium.com/max/875/1*Xokk6XOjWyIGCBujkJsCzQ.jpeg)