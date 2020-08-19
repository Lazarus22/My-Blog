---
layout: post
title:  "How I Made This Post"
date:   2020-08-17 19:31:26 -0400
categories: jekyll update
---

![My helpful screenshot](/assets/snake.jpg)
All right. I thought for this week's blog post it would be fun to do a blog about making a blog. So this post is about how this post was made. 

So one thing I think is interesting are static sites.

Static sites are often one of the first things web developers learn how to do, and they're often glanced over fairly quickly. To be moved on to more interesting and dynamic things. But static sites are actually pretty cool. Looking back, they have well developed communities, and they're worth your time. They're not just a stepping stone to do more interesting things.

So, some benefits of static site are they are fast and secure, posting can be inexpensive or completely free. One can track and coordinate versioning with GitHub. And they exist outside of content management frameworks which are between the user and the HTML you're trying to share.

What are static sites good for?

Blogs often work great for this, which is one reason I chose this project.

They do well with documentation. So, how something works, which doesn't need to be updated frequently.

Finally informational sites or brochure sites, so everything from a restaurant's menu site to just showing off a product or something along those lines.

So to build a static site it helps to have a static site generator, I went to [https://staticsitegenerators.net/](https://staticsitegenerators.net/) and you'll see its a deep rabbit hole.

![My helpful screenshot](/assets/screenshot.jpg)

One the most popular ones that's also Ruby based is called [Jekyll](https://jekyllrb.com/), Jekyll is what I'm going to be using to build my site. Jekyll is a static site generator created using Ruby and installed with a Ruby gem. It's very similar to Rails. Except, unlike Rails, its focus is only static sites. So, while its abilities are more limited, they are at the same time a bit more user friendly in that they have a smaller scope.

I got this Jekyll site up and running in 90 minutes with no experience in Jekyll. If you're familiar and comfortable with basic Rails concepts, then you're not gonna have any trouble with Jekyll, Jekyll is significantly more pared down and focused. I found the official Jekyll documentation quite thorough but in conjunction with this [Jekyll cheat sheet](https://learn.cloudcannon.com/jekyll-cheat-sheet/) and a copy of [O’reilly’s](https://www.oreilly.com/library/view/working-with-static/9781491960936/) *Working With Static Sites* I had more than enough information to sail though this quickly.  

I had an empty project open in VS code and I typed, `gem install jekyll` into the terminal. Once that was up and running, I typed `jekyll` to ensure it was installed correctly. To begin a new Jekyll project I wrote `jekyll new project_name`. That generated all the file structure in the same way running `rails new project` generates it’s own file structure. This theme you see is the default theme that Jekyll installed, but there are other more rubust themes that can be used. Jekyll uses markdown and HTML for posts but markdown is a bit simpler, and for my purposes, perfectly sufficient.

Like Rails, once that was all built I typed `jekyll s` to get the server running, and I could see my Jekyll server, instead of localhost 3000, mine was at a local IP address, but in terms of building it was a very similar process.

What's interesting about Jekyll is one of its built in properties because it's designed specifically for bloggers, so every new post file you create you name it with a date, is automatically titled it and indexed it properly without there being any work with controller files. So once that was done, I have my Jekyll file up and running, I have my project going and my servers spinning so then it was just a matter of getting the content written.

By way of generating content I use otter.ai to record this text. I went back through and formatted the text in google docs. Then formatted the links and code snippets in an online markdown editor [https://stackedit.io/app#](https://stackedit.io/app#) that let me see the changes I made live side by side with what I was doing. Once that was done I copied that over to vs code. Now I needed to deploy the site.

There are a variety of ways to deploy. The cool thing about Jekyll and deployment is that Jekyll works with GitHub. So, essentially, because GitHub is already hosting all of our files online all you need is a third party site look at your GitHub repository and build it as a website. 

There are a host of hosts. And you can if you want you can do it this manually. I did some research, and because I wanted to build this as efficiently as possible. I found a host called [netlify](https://www.netlify.com/) known for its simplicity. Netlify, allows you link to the GitHub repository of the website that you want to host. You can buy custom domains or you can just use the free built in domains that are just slightly less aesthetically pleasing, which is what I went with.

So what's cool about this is because netlify is looking at my GitHub repository, so every time I want to update my blog, I just use `git push` to my master branch, or I can just edit a post in github itself, it will update the live site. And that's the how we got here. Thank you for your time.

