# Get Ready for 401 

## Solving Problem 


**A simple set of steps** 

* Read the problem completely twice 

This is the single most important step.  You may even want to read the 

problem 3 or 4 times.

You want to make sure you completely understand the problem.  A good

 test of this is whether or not you can explain the problem to someone 
 
 else.

* Solve the problem manually 

Programming is automation plain and simple.  You may have the ability to

 skip the manual steps and jump directly to code, but there is a manual
 
  process which is the foundation of any code you write.

It is very important to solve the problem manually first, so that you 

know what you are going to automate, otherwise you are just slinging 

code around.  Which while can be fun, will make you look like an idiot 

in a programming interview and will probably cause you to sweat 
profusely.

* Optimize the manual solution 

People often don’t realize how valuable this step is.  It is much easier to rearrange and reconstruct and idea or algorithm in your head than it is in code.

It’s well worth the effort to try and optimize the actual solution or simplify it when it is still in the most easily malleable state.

What you want to do here is figure out if there is another way you can solve the problem easier, or if there are some steps you can cut our or simplify.

Let’s look at our string reversal example and see if we can simplify the steps.

We should be able to immediately recognize that we can use a loop here to reduce the manual steps.  Our duplicate why’s for most of our steps tell us that we are doing the same thing over and over for each step, just with different data.

1. Write “Zebra” down.

2. Start at the last letter in the word and create a new empty word.

3. Append the current letter to the new word

4. If there is a previous letter, make the previous letter the current letter and start back at 3.

Look how close we are getting to code at this point.  You should be tempted to actually write the code for this.  That is good, it tells you that you have solved and simplified the problem well.  Writing code should now become very easy.

* Write pseudo-code or comments 

Many times you can skip this step if you have a really good handle on the problem or your previous steps already created a detailed enough description of the solution that coding it is already a 1 to 1 translation.

If you are a beginner or struggle with these kinds of problems, I would go ahead and take the time to do this step anyway though.

* Replace comments with real code
 
 This step should be extremely easy at this point.  If you have done all the other steps, this step involves no problem solving at all.

All we do here is take each comment and convert it into a real line of code.

Taking the string reversal, we might end up with something like this.

* Optimize the real code 

Sometimes this step isn’t necessary, but it’s worth taking a look at your code and figuring out if you can cut out a few lines or do something simpler.

This is also a good place to make sure all your variables are named with long meaningful names.  I cannot stress enough how important having good names for your variables and methods is for helping the person evaluating your code to understand what you were trying to do.  This is especially important when you make a mistake!

![img](https://www.7pace.com/wp-content/uploads/2021/03/02-Image-2-scaled.jpg)

## Act like you make $1000/hr 

“Pretend your time is worth $1,000/hr. Would you spend five of them doing extra work for free? Would you waste one on being angry?” -
Niklas Göke

You have very few hours here on on this earth.

Still, many people waste much of their time on pointless, low-quality activities that don’t help them reach their true goals — their mission.
The truth is, most people value their time at far, far less than it’s worth.

They say yes to things they have no business doing. They give away their talents, attention, and effort to others who take, take, take.
They spend hours watching low-quality television and social media when they should be productive and effective.

See, many people could be making a fortune (if they used their time well)…but instead, they give away their time in unproductive ways that leave them broke, unhappy, and stuck.

But what if you placed a high value on your time?

How would that change you? Your life? Your family? Your future?

Imagine that an hour of your time is worth $1,000.

What would your life look like?

What people would you stop putting up with?

What problems would you stop wasting time on?

What things would you stop — and start — doing?

Your results would be incredible. You’d become exponentially more productive, focused, and effective.

## How to think like a programmer 

If you’re interested in programming, you may well have seen this quote before:

“Everyone in this country should learn to program a computer, because it teaches you to think.” — Steve Jobs
You probably also wondered what does it mean, exactly, to think like a programmer? And how do you do it??

Essentially, it’s all about a more effective way for problem solving.

In this post, my goal is to teach you that way.

By the end of it, you’ll know exactly what steps to take to be a better problem-solver.

Why is this important?
Problem solving is the meta-skill.

We all have problems. Big and small. How we deal with them is sometimes, well…pretty random.

Unless you have a system, this is probably how you “solve” problems (which is what I did when I started coding):

Try a solution.

If that doesn’t work, try another one.

If that doesn’t work, repeat step 2 until you luck out.

Look, sometimes you luck out. But that is the worst way to solve problems! And it’s a huge, huge waste of time.

The best way involves a) having a framework and b) practicing it.

“Almost all employers prioritize problem-solving skills first.
Problem-solving skills are almost unanimously the most important qualification that employers look for….more than programming languages proficiency, debugging, and system design.

Demonstrating computational thinking or the ability to break down large, complex problems is just as valuable (if not more so) than the baseline technical skills required for a job.” — Hacker Rank (2018 Developer Skills Report)

![img](https://media.geeksforgeeks.org/wp-content/cdn-uploads/20200326191711/How-to-Think-Like-a-Programmer.png)

## 5 Whys 

**How to Use the 5 Whys** 

The model follows a very simple seven-step process:

1. Assemble a Team
Gather together people who are familiar with the specifics of the problem, and with the process that you're trying to fix. Include someone to act as a facilitator , who can keep the team focused on identifying effective counter-measures.

2. Define the Problem
If you can, observe the problem in action. Discuss it with your team and write a brief, clear problem statement that you all agree on. For example, "Team A isn't meeting its response time targets" or "Software release B resulted in too many rollback failures."

Then, write your statement on a whiteboard or sticky note, leaving enough space around it to add your answers to the repeated question, "Why?"

3. Ask the First "Why?"
Ask your team why the problem is occurring. (For example, "Why isn't Team A meeting its response time targets?")

Asking "Why?" sounds simple, but answering it requires serious thought. Search for answers that are grounded in fact: they must be accounts of things that have actually happened, not guesses at what might have happened.

This prevents 5 Whys from becoming just a process of deductive reasoning, which can generate a large number of possible causes and, sometimes, create more confusion as you chase down hypothetical problems.

4. Ask "Why?" Four More Times
For each of the answers that you generated in Step 3, ask four further "whys" in succession. Each time, frame the question in response to the answer you've just recorded.

Step 5. Know When to Stop

You'll know that you've revealed the root cause of the problem when asking "why" produces no more useful responses, and you can go no further. An appropriate counter-measure or process change should then become evident. (As we said earlier, if you're not sure that you've uncovered the real root cause, consider using a more in-depth problem-solving technique like Cause and Effect Analysis , Root Cause Analysis , or FMEA .)

If you identified more than one reason in Step 3, repeat this process for each of the different branches of your analysis until you reach a root cause for each one.

6. Address the Root Cause(s)
Now that you've identified at least one root cause, you need to discuss and agree on the counter-measures that will prevent the problem from recurring.

7. Monitor Your Measures
Keep a close watch on how effectively your counter-measures eliminate or minimize the initial problem. You may need to amend them, or replace them entirely. If this happens, it's a good idea to repeat the 5 Whys process to ensure that you've identified the correct root cause.

 

![img](https://www.mindtools.com/media/Diagrams/5_Whys_Figure_1_Single_Lane.jpg)

