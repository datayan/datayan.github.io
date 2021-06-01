---
layout: post
title: Using Atom With Markdown For A Blog On GitHub Pages
---

![github-atom-markdown](/images/github-atom-markdown.png)

Atom is a phenomenal free code editor. The plethora of extentions for it makes it a real pleasure to play with and experiment. Among it many many features that I am still finding out after using it for a the better part of the year, is its capability to handle Markdown. After using many platforms and editors for my blog needs, I found the combination of GitHub, Atom and Markdown the best suited for me. Lightwight, geeky and tremendously simple and it makes me somehow feel like I am still coding and not really writing a blog post. But thats just me.

###### So what exactly is GitHub ?

![github](https://github.githubassets.com/images/modules/site/home/repo-browser.png)
Just in case you are not aware, GitHub is the worlds largest host for source code, hosting almost 200,000,000 repositories. Owned by Microsoft, it offers the distributed version control and source code management (SCM) functionality of Git, plus its own features. It provides access control and several collaboration features such as bug tracking, feature requests, task management, continuous integration and wikis for every project. In other words, if you are writing code, heaad on over to Github and start saving your code there. In addition to these features GitHub has a feature called GitHub Pages, which can be used to hosts simple websites like portfolios, blogs, project information etc.

###### So what exactly is Atom ?

![atom](https://user-images.githubusercontent.com/378023/49132478-f4b77680-f31f-11e8-9e10-e8454d8d9b7e.png)

Atom is a free and open-source text and source code editor for macOS, Linux, and Microsoft Windows with support for plug-ins written in JavaScript, and embedded Git Control, developed by GitHub. Atom is a desktop application built using web technologies. Most of the extending packages have free software licenses and are community-built and maintained. Atom is based on Electron (formerly known as Atom Shell),a framework that enables cross-platform desktop applications using Chromium and Node.js. Its developers call it a "hackable text editor for the 21st Century", so it is meant to be customized till you drop dead.

###### So what exactly is Markdown ?

![markdown](https://res.cloudinary.com/practicaldev/image/fetch/s--4JbB7SY9--/c_imagga_scale,f_auto,fl_progressive,h_420,q_auto,w_1000/https://dev-to-uploads.s3.amazonaws.com/i/g595slgphyi9lkqz2u18.png)
Markdown is a lightweight markup language for creating formatted text using a plain-text editor. John Gruber and Aaron Swartz created Markdown in 2004 as a markup language that is appealing to human readers in its source code form. Markdown is widely used in blogging, instant messaging, online forums, collaborative software, documentation pages, and readme files. Simply, its a way to type your text like you do for code. Geeky !!

###### So how did I go about using these tools to start a blog?

![jekyll](https://repository-images.githubusercontent.com/65252/f2b7c780-70b6-11e9-85d2-f4bda8708a2d)

I started by forking a Jekyll setup called [Jekyll-Now][701ca9b6] on Github and renaming that repo to myusername.github.io. That would be the home of my blog. Thats exatly where we are right now.

  [701ca9b6]: https://github.com/barryclark/jekyll-now "Jekyll-Now"

For the uninitiated, Jekyll is a simple, blog-aware, static site generator for personal, project, or organization sites. The authors very simply state that, "Jekyll does what you tell it to do — no more, no less. It doesn't try to outsmart users by making bold assumptions, nor does it burden them with needless complexity and configuration. Jekyll gets out of your way and allows you to concentrate on what truly matters: your content". Good enough.

Once the repo was alive and the test site online which usually takes around 10 minutes. I pulled the repo using GitHub Desktop and made a local copy. Opened the local copy on Atom by opening a project. From the tree view I made my way to the "_posts" folder. This is the home of the all the text files / markdown files which will be each individual post. The files here end in the extention '.md' which stands for markdown.

We do need to keep in mind that Jekyll likes the posts to be be in the format "yyyy-mm-dd-title-post.md", otherwise it will not build the static page. While writing the body of the text, I had to brush up on the Markdown sysntax. This markdown [guide][2dcd77b5] proved to be extremly helpful for this task.

  [2dcd77b5]: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet "Markdown Guide"

Another thing to keep in mind which will help avoid build errors is the header text for each post,

```markdown
---
layout: post
title: your post title
---
```
After I wrote the content, I saved the file and pushed my changes to Github all through Atom. Viola in a few minutes this page was alive on the username.github.io. domain.

So this is how I am using GitHub, Markdown and Atom to write my blog. I shall be updating this page as I tinker around this workflow even more. So far this has been a great expereince.

Many many thanks to the article by Barry Clark for this rather amazing way to set up the blog. [[Full Article]](https://www.smashingmagazine.com/2014/08/build-blog-jekyll-github-pages/)
