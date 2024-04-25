---
layout: post
title: "How to build my simple GitHub Blog and Posts"
date: 2024-04-25
---
I have to say creating a blog was the main objective of one of my assignment question, but more so, it was to facilitate better ongoing learning like I said in previous post. Creating a blog allows for the organization of many thoughts during the learning process, 
which can be reviewed later. This includes the current assignment, and I will subsequently post about some of the difficulties I encountered while creating a GitHub blog.  

The primary steps for creating the GitHub blog page were to follow the instructions provided by [fast.ai], these steps included creating an account, setting up repositories,
and crafting posts. However, I encountered some issues while following the instructions.  

For example, when trying to name the repository as my username instead of using `username.github.io`, which led to problems when creating the `_config.yml` and `index.md`,
then I attempted to set a title and description in the `_config.yml` and texting the content in the `index.md` for testing, however, I found that only the content from the `index.md` was displayed, and when trying to access my GitHub blog page, it showed a 404 Not Found error.  

I spent some time troubleshooting this issue, including looking for tutorials on YouTube to help with the setup. Since I had no prior experience in web development, I often confused markdown code with HTML code in the tutorials.  

In my final blog, I opted for the theme called Minima, similar to [Professor Brian's Blog]. Minima was also used in the [fast.ai] instructions and many YouTube tutorials, 
allowing me to plan the blog content and template based on the provided sample blogs. Later, I found the [original files] provided by jekyll on GitHub, which made it easier for me to consult and learn the code needed for better formatting.  

I also encountered several issues along the way. The initial problem was setting up a homepage title like Brian's "Blog". When trying to create a series of titles using hashtags as suggested by fast.ai  
  {% highlight ruby %}
  ## Blog
  Hello, this Lawrence, a Master student studying electrical engineering at the University of Queensland, I finished my Bachelor degree in University of New South Wales.  
  Here will post the work I have done before and also, show some work I'm doing right now.  
  Hope you guys enjoy it~
  {% endhighlight %}
the generated HTML on GitHub showed duplicate titles and no line break:  
<img src="_posts/images/1b.jpg"/>  
I also encountered issues with line breaks, initially tried to solve these issues using LaTeX methods but it did not work, 
then sought a line-break equivalent in LaTeX and learned how to create titles by studying minima's original files. After learning from these original source files, I understood how to post an article, add images, and list items using `\begin{itemize}` in LaTeX, enabling me to better format my blog and more quickly build my own.  

Here is the final code for solving this question:  
  {% highlight ruby %}
  ---
title: "Blog"
---

Hello, this is Lawrence...<br>
  {% endhighlight %}

Maybe I will write another post on how to make the homepage more fashionable, but not now...  

Cheers,  
Lawrence  
<img src="/images/smile.jpg" width="300" />

[fast.ai]: https://www.fast.ai/posts/2020-01-16-fast_template.html.
[Professor Brian's Blog]: https://lovellbrian.github.io
[original files]: https://github.com/jekyll/minima/tree/master
