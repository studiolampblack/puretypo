---
layout: page
title: Help
navigation: True
logo: 'assets/images/merakipost.svg'
current: help
cover: 'assets/images/cover1.jpg'
permalink: /help/
indexing: false
---

> This is a Meraki Post internal page, to help us with the common formatting guidelines, so as to ensure uniformity throughout the site. This page may not be relevant to you if you're a visitor.

Posts on this site are made using this beautifully simple lightweight markup language called *Markdown*. This is so that you can use any text editor (including the good old Notepad), to write posts.

### The basics

1. Every post you make is essentially a markdown file, which looks like a text file.
2. All posts must be placed in the folder, `_posts`.
3. All drafts must be placed in the folder, `_drafts`.
4. All posts you place in the `_posts` folder should be named like `2017-09-30-name-book.md`.
5. All posts should have the following *frontmatter* in the beginning of the file (including the three hyphens).

{% highlight yaml %}
---
layout: post
title: Name of the Book
subtitle: Name of the Author
date: 2017-09-30
author: yourname
tags:
- tag1
- tag2
- tag3
image: assets/postimages/imagename.jpg
---
{% endhighlight %}

### General guidelines

1. When naming files, omit non-catch words. For instance, `Alice in Wonderland` would become, `alice-wonderland`; this is called *slugification*.
2. The date should be in `yyyy-mm-dd` format, such as `2017-04-15`.
3. Therefore, the filename would be a combination of the date and the title, separated by a hyphen, such as `2017-04-15-alice-wonderland`.
4. The `layout` should be `post`, and only `post`.
5. The title should be a full title, with proper capitalisation.
6. The subtitle should be the full name of the author, appropirately capitalised.
7. The `author` attribute here is for the author of the post, which is you. Write your first name, all in lowercase, such as, `ram`.
8. Tags are important. Make sure you leave the `tags:` line empty, and list down the tags preceded by a hyphen and a space, followed by the tag. Tags can have spaces. So, it's OK to have a tag like `historical fiction`.
9. Image is important, too. It is typically the cover image. *Compress the image*, and store it under `\assets\postimages` as a JPG file. Add the link to that image here, replacing `\` with `/`. Windows understands `\`, Jekyll doesn't.
10. Most importantly, don't forget to enclose this content between two lines of three hyphens (`---`) each.

Here's a complete sample to help you understand.

{% highlight yaml %}
---
title: The First Trillionaire
subtitle: Sapna Jha, translated by Alok Jha
date: 2017-05-20
tags:
- fiction
- thriller
image: assets/postimages/firsttrillionaire.jpg
author: ram
---
{% endhighlight %}

### Formatting the posts

Formatting content is very easy with markdown. Here are the different formats we have:

#### Paragraph

1. Just type on, like you would on Word. Make sure you don't make spelling or grammatical errors.
2. Leave a blank line after the frontmatter.
3. Leave a blank line after every paragraph.

Here's an example:

{% highlight markdown %}
tags:
- fiction
- thriller
image: assets/postimages/firsttrillionaire.jpg
author: ram
---

I'd come across this title back in 2016 when I chanced upon the site about the "Most compelling read of 2016". When I was one among the winners of the Goodreads Giveaway of this book, I was overjoyed! While I waited for the book, I went through the reviews of the book on Goodreads. At the time of checking, the book had 270 five-star ratings, out of 274. Unbelievable, but true.

Sure enough, after some days of eagerly waiting, I received the book, and I started reading it. And the journey began.
{% endhighlight %}

Notice the blank line after the frontmatter, and between the two paragraphs.

#### Cover image

Just copy-paste the following code. Liquid will take care of putting up the image, as long as you've specified the image in the frontmatter.

{% highlight markdown %}
![Cover: {{ page.title }}]({{ site.baseurl }}{{ page.image }} "Cover: {{ page.title }}")
{% endhighlight %}

#### Subheadings

Subheadings are specified using `#`. A first-level subheading is written as `# First Level Heading`. A second-level subheading is written with two hashes, like `## Second Level Heading`. The number of hashes decide the level.

The subheadings in our posts are all third level.

Also, ensure that there's a blank line before and after the subheading. Here's an example.

{% highlight markdown %}
Not one of the most thrilling covers, I had to admit. But let's not judge the book just by its cover.

### Characters

The story primarily revolves around Shail, the protagonist, of course. In scenes where the protagonist is absent, the focus promptly shifts to the other important characters.
{% endhighlight %}
