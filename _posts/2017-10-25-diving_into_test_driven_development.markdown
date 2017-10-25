---
layout: post
title:      "Diving into Test-Driven Development"
date:       2017-10-25 13:37:06 -0400
permalink:  diving_into_test_driven_development
---


At my online coding school, Flatiron School, we are introduced to the main concepts behind Test-Driven Development (TDD) briefly, but we use tests on every lab we encounter. Only, the tests are already written for us as guidelines for how to correctly complete a lab. Once we fork and clone our labs, we run our tests, and they are failing. It is our job as students to make them pass. Once they pass, “Congrats, you’ve finished your lab!”


![](https://media.giphy.com/media/QW5nKIoebG8y4/giphy.gif)


However, I have never actually done test-driven development myself, that is, until this month when I was completing a coding challenge. And let’s face it, writing tests from scratch (especially with it being the first time) was a little bit daunting. However, TDD is something that I am looking forward to working with as I transition from student to full-time developer, so I was excited and up for the challenge! I feel like I learned a lot throughout this process, but I know I have a long way to go before I become a TDD wizard. 

Before I started writing my tests and code, I watched some tutorials and read some articles on TDD and using RSpec (since I was coding in Ruby, I used RSpec for testing). Then, I set up my project and dove in!

At first, it took me a while to think of what tests to write next and how best I could write them. But once I got the hang of writing them (or at least how I thought they were supposed to be written), it became more of a habit. I didn't think in terms of, "what code I needed next to solve this problem," but instead I thought, "what do I have to test next to get my problem working." And this all falls into TDD's approach of Red-Green-Refactor. First, you write a test that would help solve your next problem. When you run your tests, it is "red" because it is failing -- you have no code written yet to solve this! So, you move onto the "green" step and begin writting code to make your test pass. Once your test is passing, you can look back at your code and "refactor" if neccessary. And trust me, it is really fun to see your tests go from red to green!


![](https://media.giphy.com/media/vBCGCW5o8FPjy/giphy.gif)


Throughout the process of completing my test-driven challenge, I noticed some benefits of TDD. First of all, using TDD gave me confidence that my code was actually working as intended. As long as your test is written correctly, once you are able to get a red test to turn green, most of the time, you can safely assume that the code your wrote is working like you wanted and you are ready to move on to the next step. This is great, because you get feedback on whether your code is working or not in a very short amount of time and you are not wasting time writing a bunch of code when something 5 lines ago was broken.

Another thing I love about TDD is that it lets you know if the code you are writing now is breaking any previously working code you wrote in the past. If this is happening, some of the older tests you wrote would turn red right away, letting you know that something isn't working properly. This makes it easy for you to notice a problem and fix it quickly.

Lastly, another major thing I like about TDD is that in the end, you have a story about how your code should be working. In a way, writing tests is like documenting or commenting your code, it is just in a different file and also includes tests or examples on how your code should behave.

There are many more benefits to using TDD, but this blog may get too long if they were all included. These are just a few of the big ones that I noticed my first time doing test-driven development. With all the benefits that come with TDD, I think it is worth the initial investment it requires to learn how to write the tests. Like with most new things we try out, I feel like overtime, as I practice and improve on my TDD skills, writing tests will become quicker and more second nature.

My goal is to continue to practice TDD as I transition from being a student to a professional developer. Since this was my first time doing TDD, I am still unsure if I am writing my tests correctly or using the best practices I can be using. However, I am hoping that as I continue to practice and explore TDD more in the future, I will be able to improve my test writing and my TDD skills overall!


![](https://media.giphy.com/media/7MZ0v9KynmiSA/giphy.gif)


