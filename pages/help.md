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

Posts on this site are made using this beautifully simple lightweight markup language called *Markdown* (I know, Markdown markup sounds funny). This is so that you can use any text editor, including the good old Notepad, to write posts.

Tools you need:

1. [Atom by GitHub](https://atom.io/) to write posts in a beautiful interface.
2. [RIOT by Lucian Sabo](http://luci.criosweb.ro/riot/download/) to compress images for the posts so things load superfast.
3. [GitHub for Windows by GitHub](https://desktop.github.com/) to push content to GitHub.

### The basics

1. Every post you make is essentially a Markdown file, which looks like a text file.
2. All posts must be placed in the folder, `_posts`.
3. All drafts must be placed in the folder, `_drafts`.
4. All posts you place in the `_posts` folder should be named like `2017-09-30-name-book.md`.
5. All posts should have the following *frontmatter* in the beginning of the file (including the three hyphens).

{% highlight text %}
---
layout: post
title: Name of the Book
subtitle: Name of the Author
date: 2017-09-30
author: yourname
tags:
- tag1
- tag2
image: assets/postimages/imagename.jpg
---
{% endhighlight %}

### General guidelines

1. When naming files, omit non-catch words. For instance, `Alice in Wonderland` would become, `alice-wonderland`; this is called *slugification*.
2. The date should be in `yyyy-mm-dd` format, such as `2017-04-15`.
3. The filename would be a combination of the date and the title, separated by a hyphen, along with its extension, `.md` (for Markdown), such as `2017-04-15-alice-wonderland.md`.
4. The `layout` should be `post`, and only `post`.
5. The title should be a full title, with proper capitalisation.
6. The subtitle should be the full name of the author, appropirately capitalised.
7. The `author` attribute here is for the author of the post, which is you. Write your first name, all in lowercase, such as, `veena`.
8. Tags are important. Make sure you leave the `tags:` line empty, and list down the tags preceded by a hyphen and a space. Tags can have spaces. So, it's OK to have a tag like `historical fiction`.
9. Image is important, too. It is typically the image of the book cover. *Compress the image*, and store it under `\assets\postimages` as a JPG file. Add the link to that image here, replacing `\` with `/`. Windows understands `\`, Jekyll understands `/`.
10. Most importantly, don't forget to enclose this content between two lines of three hyphens (`---`) each.

Here's a complete sample to help you understand. Note that there's no `by` before the name of the author.

{% highlight text %}
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

Formatting content is very easy with Markdown. Here are the different formats we have:

#### Paragraph

1. Just type on, like you would on Word. Make sure you don't make spelling or grammatical errors.
2. Leave a blank line after the frontmatter.
3. Leave a blank line after every paragraph.

Here's an example:

{% highlight text %}
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

### Poem verses

Poem verses require line breaks, and not paragraph breaks, when splitting lines. To achieve this, put a double `\`, at the end of each line you need a line break at, like so:

{% highlight text %}
Mommy had a little calf.\\
Little calf.\\
Little calf.\\
Mommy has a little calf.\\
His nose is black as tar.
{% endhighlight %}

Remember not to add the `\\` markup at the end of the last line of the stanza.

#### Cover image

> Compressing the image is important.

Just copy-paste the following code. Liquid will take care of putting up the image, as long as you've specified the image in the frontmatter.

{% highlight text %}
{% raw %}
![Cover: {{ page.title }}]({{ site.baseurl }}{{ page.image }} "Cover: {{ page.title }}")
{% endraw %}
{% endhighlight %}

#### Subheadings

Subheadings are specified using `#`. A first-level subheading is written as `# First Level Heading`. A second-level subheading is written with two hashes, like `## Second Level Heading`. The number of hashes denote the level.

The subheadings in our posts are all third level.

Also, ensure that there's a blank line before and after the subheading. Here's an example.

{% highlight text %}
Not one of the most thrilling covers, I had to admit. But let's not judge the book just by its cover.

### Characters

The story primarily revolves around Shail, the protagonist, of course. In scenes where the protagonist is absent, the focus promptly shifts to the other important characters.
{% endhighlight %}

#### Block quotes

Block quotes are your favourite formatting control from the Blogger Editor and Open Live Writer. This is used to produce formatting just how it is at the beginning of this page. In Markdown, it is very simple. Just precede the text with `>`. A space after `>` is optional. However, to make the style consistent, you may want to add a space after the `>`. Technically, that will have no effect on formatting whatsoever.

{% highlight text %}
> Run as fast as you can and tell Gopal to come here with Dr Narayan. And also go and tell Mr Singh to come here. He stays next to me.
{% endhighlight %}

What you need to remember here is that if you want to separate block quotes, you need to leave an empty line between the block quotes that you want separated.

#### Emphasis

Emphasis usually is shown using _italics_ in books. It is more about the kind of font we're using. We use a serif font, called Crimson Text. In this case, it is good to use italics, since this font has real italics, and they're distinct from the roman (normal) style.

To emphasise any text, wrap it between two `_`, just how we do it on WhatsApp. Here's an example. Here, 'at least' will be italicised.

{% highlight text %}
My high school grammar class tells me, there are _at least_ three errors in the quoted text.
{% endhighlight %}

#### Other important entities

All our content is HTML. When putting up content, especially since we're all about literature, a style guide is important. It shows that we care about quality.

Open Live Writer used to take care of those little things like an em-dash and all, when you typed. It wouldn't be the case here. We need to take a small step to ensure things are as we need them to be. It's absolutely possible, no worries.

Please follow the guidelines listed below to ensure we maintain our reputation with respect to quality:

1. Use hyphens to spell multipart words, such as, _hither-thither_. Use a hyphen with phrasal adjectives as well, such as _high-end machinery_. Writing a hyphen is as simple as typing the `-` key on the keyboard.
2. Use an _en dash_ to show ranges, or when connecting pairs of words, such as _1939&ndash;1945_, or _The India&ndash;Pakistan relationship_. An en dash is written using a pair of hyphens, like `1939--1945`.
3. Use an _em dash_ to give a nice break to the sentence you're writing, such as _Today, book typography is conveniently&mdash;and blatantly&mdash;ignored._ This is done using three hyphens, like, `Today, book typography is conveniently---and blatantly---ignored.`
4. When you want the ellipsis (&hellip;), just type three dots `...`. Markdown will convert it to an ellipsis character.
5. Non-breaking spaces are important. These ensure that things like _Dr&nbsp;Jekyll_ and _25&nbsp;km_ don't split---that's because _Dr_ at the end of a line and _Jekyll_ on the next line would make no sense. You'd need to insert a non-breaking space to ensure this doesn't happen. Enter a non-breaking space with an HTML entity, `&nbsp;`. The ampersand and the semicolon are _very important_. An example would be, `Mr&nbsp;Singh`. Also note that a non-breaking space itself is a space, so don't add an additional space before or after the entity. It'll simply kill its purpose.

#### Lists

Our site has to hardly use a list---a bulleted or numbered. However, if we do, here's how we'd do it:

{% highlight text %}
An example of numbered list would be like this:

1. First point
2. Second point
3. Third point

That's how you make a numbered list.
{% endhighlight %}

Notice the blank lines before and after the list. It is important. The list would not be rendered properly if the space is ignored.

{% highlight text %}
An example of bulleted list would be like this:

* First point
* Second point
* Third point

You could also use a hyphen, like so:

- First point
- Second point
  - A subpoint
  - Another subpoint
- Third point

Hit the `Tab` key on your keyboard for the indentation. You could also add a couple of spaces before the hyphen for indentation. Markdown can understand that.
{% endhighlight %}

#### Hyperlinks

Hyperlinks are simple. Enclose the text to show on the page in square brackets, `[like so]`, and enter the link in parentheses, like `Visit [Meraki Post](www.merakipost.com) for more exciting content!`, to get _Visit [Meraki&nbsp;Post](www.merakipost.com) for more exciting content!_
