---
layout: post
title: AI-ntrusive thoughts
lang: en
lang-ref: ai-ntusive
tags:  [ai, generative programming]
---

I recently came across the following figure, which I find quite thought-provoking.

Essentially, all the popular generative models today "learn" 
from the Internet in the broadest sense. 
A good summary of the technology itself can be found on 
[javax0](https://javax0.github.io/2024/07/22/llm-and-rag-hu.html)'s blog.

The image shows a sharp decline in StackOverflow visits and, in parallel, user activity. 
But here's the thing: the most important source of all programming-related topics 
for all these models is StackOverflow itself! 
If the content disappears from there, what will the robot learn from? 
And what will happen to future technologies?

![stackoverflow-after-chatgpt-tom-alder.jpg](/artifacts/stackoverflow-after-chatgpt-tom-alder.jpg)

This question is a bit of a chicken and egg problem, 
but it's clearly becoming more pressing now 
that even more people will use coding assistants after 
[GitHub copilot](https://github.blog/news-insights/product-news/github-copilot-in-vscode-free/)
became free.


<!-- more -->


## Personal Point of View

The above also has an impact on my own blog. 
Here, I have been trying to explore things that interest me 
or that I've encountered, but that aren't so important during work. 
And at the same time, share my own experiences and the obstacles I've faced.

Others do the same, many of whom are much more talented, 
skilled, and experienced than me. Obviously, their motivation is also reduced 
by the fact that "ChatGPT will tell you anyway." Anyone can get an immediate, 
prompt answer about anything.

Why should I write anything at all, who will even read it?

This reduces the relevant content that can be processed by the robot, 
and it settles into a fixed average quality. Managers are happy, 
until they are fired in the next wave of layoffs, 
because at a certain level they are even more easily replaced 
by a well-trained chatbot.


## Computers and the Expected Answer

I read another opinion from Tamás Sallai, and although we haven't met for a while, 
I have to agree with the issues he raised. It can be read in this post: 
[Thoughts on unreliable computing](https://advancedweb.hu/shorts/thoughts-on-unreliable-computing/), 
but he also started based on 
[Rob Bowley's post](https://www.linkedin.com/posts/robertbowley_is-computer-says-maybe-the-new-computer-activity-7272155588271255552-wfOi/).

This issue, although related to the previous one, is very different.

From the user's point of view, the expectation is very important! 
Until now, we expected a machine to give an exact answer to an exact question. 
This will no longer be the case.

Users (i.e., us) will get used to the fact that ChatGPT will give some answer, 
which is mostly true, but not certainly so. It writes a poem for 
[George Byron](https://hu.wikipedia.org/wiki/George_Byron), 
which is in his style, but he didn't write it. 
We ask it for something, and it returns something similar, 
but from a completely different perspective.


## Image generation

Image generation is another topic besides DeepFace and its kind. 
The latter are already being used in election campaigns even at a very low level. 
I was surprised that even in a small village's mayoral election campaign, 
they were used to discredit the incumbent candidate 
and spread things he never said on Facebook.
It's a strange world what's going on even on such a small scale. :)

Creating, painting, drawing a picture is a real creative activity, 
but now even a simple keyboard tapper is capable of "anything". 
First only for fun, and then soon they will overtake 
human colleagues in active content generation.

[Dall-e 3](https://openai.com/index/dall-e-3/), [Stable Diffusion](https://stability.ai/stable-image), 
and their kind have flooded the Internet, 
and by now it's really hard to tell about one or another picture 
whether a real artist is behind it, 
or just a well-parameterized generative AI spat it out.

By now, with downloadable models, anything can be produced in minutes 
even with average and cheap PC configurations. So I did too, I downloaded 
[stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui) 
plus some pre-trained models, and one picture was made after another.

Motto: "korean girl with flower in her hand"

StableDiffusion base model: 
![korean-girl-with-flower-in-her-hand-001.png](/artifacts/korean-girl-with-flower-in-her-hand-001.png)

The initial model's errors are clearly visible: the number of fingers is wrong, 
the flowers are not (only) in her hand, the lines are mixed up at the mouth. 
But it is still basically recognizable.

Then, with the help of [Google Gemini](https://gemini.google.com), 
I could ask for something else.

This was the prompt: "Generate an image of a rainbow-colored eight-headed cat."

Gemini 1.5 Flash model:

![Gemini_Generated_Image_q4bt3rq4bt3rq4bt.jpg](/artifacts/Gemini_Generated_Image_q4bt3rq4bt3rq4bt.jpg)

The same with Gemini 2.0 Flash beta model:

![Gemini_Generated_Image_q4bt3rq4bt3rq4bt.jpg](/artifacts/Gemini_Generated_Image_v8vh5xv8vh5xv8vh.jpg)

Well... It still can't count, although the newer model has reached from three to six, 
but [Bel-Shamharoth](https://discworld.fandom.com/wiki/Bel-Shamharoth)
seems to scare even a robot.

## Closing Words

Although this post has become a bit scattered and not entirely positive, 
no one (robots included) should take it personally.

__Happy New Year!__


*** translation aimed by Google Gemini