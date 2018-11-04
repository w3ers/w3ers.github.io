---
title: jQuery Number Converter
date: 2018-11-04 16:14:11 +0000
undefined: []

---
If you run a blog that is in other language than English, such as indic languages or Semitic languages, you probably face problem of showing the numbers in your native language. I have several WordPress blog in Bangla. I struggled a lot to find an easy way to convert English number characters to Bangla. But, there was not a single plugin that can do the job properly. Then I wrote a few lines of code in jQuery and the problem was solved! The good thing is this tiny code snippet will work on any website.

Let's dive into the code.

At first let's mock-up a pseudo code that explains how our original code will work.

First, we have to say or declare the characters of our native language. In this case, it is Bangla. Banla number characters are-  ০ (0), ১ (1), ২ (2), ৩ (3), ৪ (4), ৫ (5), ৬ (6), ৭ (7), ৮ (8), ৯ (9).

So, we will declare a list that contains all the charters.

Then we declare a list of selector, classes or id's where the changes need to be applied. Then what?

Then we will build a process that replaces all the English numbers into Bangla ones. It will work as follows-

1\. Go to each selector we listed.

2\. Split every character.

3\. Find numbers in there.

4\. Find the character of that numbers position in the declared native numbers list.

5\. Replace English character with that non-English character.

6\. Join split text again.

Now, Let's look at the jQuery code to get this job done.

<iframe allowfullscreen="true" allowtransparency="true" frameborder="no" height="265" scrolling="no" src="//codepen.io/utsargo/embed/zMYQXP/?height=265&theme-id=0&default-tab=js,result" style="width: 100%;" title="jQuery Number Converter">See the Pen <a href='https://codepen.io/utsargo/pen/zMYQXP/'>jQuery Number Converter</a> by utsargo (<a href='https://codepen.io/utsargo'>@utsargo</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

Paste the JavaScript code before "</body>" tag of your page. You can replace the variable bengaliNumbers with anything you want, and replace the number characters with your own list. Put your desired selector list separated with comma in selectorList. That's it. You are ready to go.

### How to implement in WordPress 

If you want to use this code in WordPress, you will need a custom JavaScript plugin. There are a few of them. Use one to implement the code.