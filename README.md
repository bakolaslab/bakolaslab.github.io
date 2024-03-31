# Bakolas lab page

This is repository for [Bakolas lab page](http://bakolaslab.github.io/). We use Jekyll to run our Github page. We are welcome for other people to contribute to our site not just lab members. Feel free to fork and pull-request!

## Getting Started

First, you need to clone the repository to your local machine. You can do this by running the following command in your terminal:

```bash
git clone https://github.com/bakolaslab/bakolaslab.github.io.git
```

Then, you need to install Jekyll. If you are using Ubuntu, you can install Jekyll by running the following command:

```bash
sudo gem install jekyll
sudo gem install rouge
jekyll serve
```

If not, follow instructions [here](https://jekyllrb.com/) to install Jekyll then run `jekyll serve` to see in `localhost:4000`.

Once done with your changes, you can push your changes to the repository by running the following commands:

```bash
git add .
git commit -m "Put your message here (i.e. what changes you made)"
git push origin main
```

To avoid having conflicts, it is **highly recommended** make sure that you pull the latest changes from the repository before you make any changes. You can do this by running the following command:

```bash
git pull origin main
```

## Editing the lab website

Below, we explain how to edit the lab webpage

### Add yourself

You can add yourself to the page in `_people` folder just create file name `<firstname>_<lastname>.md` in the folder. We require few line of header before you start writing your own page. See the following for the header

``` markdown
---
name: Eva Dyer
position: postdoc
avatar: eva.jpg
twitter:
joined: 2014
---
```

If you don't have information, just leave it blank. The avatar will bring photo from `images/people` folder and display it on people page. 
For lab position, you can choose position from 4 classes including `postdoc`, `gradstudent`, `visiting`, `others` (so called Honorary members). Position will put you into section that you choose.

### Add new publications

All publications from the lab are located in `publications.md`. Please upload new publication on your own!

### Add news

All news presented in the front page by editing `_data/news.yml`. There are some symbol that cannot be used directly e.g. `:`, be careful


### Add posts

It's very easy to add post. All the posts are located in `_posts` folder. It arrangement is based on
date. Each post can be written in markdown format. You just have to state headers before writing: `title`, `description` and `categories`. `description` will be shown when you share on social media like Facebook or twitter. See the following headers:

``` markdown
---
title: Summer School in Computational Sensory-Motor Neuroscience (CoSMo)
description: all links to CoSMo summer school in computational neuroscience materials
categories: scientists
---
```

We have 4 categories: `scientists`, `students`, `discussion`, `blog` you can choose and this will be rendered to different location.

### How to add posts

- **Directly edit on Github**, you can simply go to `_posts` and click `New file` then put some markdown file e.g. `2016-02-03-post-name.md` and start writing blog post. Github also allows you to preview it so it's nice for people who don't want to clone the repo. 

- **Clone the repository**, kind of the same as directly add post on Github. You just have to clone the repository. Then add new post file, commit and push to the repo.

The changes will take approximately half a minute to render. You can see the new posts or changes on [bakolaslab.github.io](http://bakolaslab.github.io/)!