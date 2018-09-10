# How to contribute

Thank you for contributing to the [Ohio Suffrage Centennial](https://www.ohiosuffragecentennial.com/) website! We're glad you're here and appreciate your help.

This document describes our goals with the website, a few special HTML and Markdown conventions, and how to submit your changes,.

## Goals

With this website, we hope to inspire people to:
* Plan something (anything!) during 2019 and 2020, the years that mark the 100th anniversary of women's right to vote in the United States
* Learn about Ohio's incredible connections to women's fight for equal suffrage and the 19th amendment
* Find out about events and sites throughout Ohio and the United States that are connected to the woman suffrage movement

We want to guide people to existing resources and information.

## Content overview

The website contains five pages: Home, Plan Something, Learn Something, News, and Contact. We welcome contributions for the Plan Something and Learn Something pages and posts to the News page.

The [Plan Something](https://github.com/OhioSuffrageCentennial/ohiosuffragecentennial/blob/gh-pages/plan.html) page lists websites that have information about locations and events related to woman suffrage history.

The [Learn Something](https://github.com/OhioSuffrageCentennial/ohiosuffragecentennial/blob/gh-pages/connections.html) page lists information highlights about Ohio's significance to woman suffrage history.

The [News](https://github.com/OhioSuffrageCentennial/ohiosuffragecentennial/blob/gh-pages/news.html) page is a collection of [brief posts](https://github.com/OhioSuffrageCentennial/ohiosuffragecentennial/tree/gh-pages/_posts) about 19th-amendment-related events, especially those held or planned in Ohio.

## Frontmatter

You may have noticed content at the top of the website files between two `---` marks. This is structured [`yaml`](http://yaml.org/) data that Jekyll uses to get more information about the file, such as the `<title>` of the page, the publication date, and more. This is referred to as **`frontmatter`**.

All of the website pages and posts include Jekyll frontmatter. **Do not** change the frontmatter in the Plan Something, Learn Something, or News pages. **Do** alter the front matter for News post contributions as described below.  

### News post frontmatter

All [posts](https://github.com/OhioSuffrageCentennial/ohiosuffragecentennial/tree/gh-pages/_posts) for the [News](https://github.com/OhioSuffrageCentennial/ohiosuffragecentennial/blob/gh-pages/news.html) page must begin with the following frontmatter:
```
---
layout: post
title: Title of post in sentence case
date: YYYY-MM-DD HH:MM:SS
author: Ohio Suffrage Centennial
---
```

Replace the placeholder values for the `title` and `date` with information that is specific to your post. Do not change the `layout` and `author` values.

## Editorial style

We use US English and try to write plainly and conversationally.

## File and directory conventions for News posts

Save all News posts to [https://github.com/OhioSuffrageCentennial/ohiosuffragecentennial/tree/gh-pages/_posts](https://github.com/OhioSuffrageCentennial/ohiosuffragecentennial/tree/gh-pages/_posts).

If you create a new `posts` file to add to the documentation, please follow these file-naming conventions:

* Begin with the date in `YYYY-MM-DD` format
* Lower-case only
* Hyphens between words (for example, `case-study`, not `casestudy` or `case_study`)
* Include the `.md` file extension

For example:
```
YYYY-MM-YY-post-title-lower-case.md
```

## Link format

Use HTML format to create links in website content, including `target="_blank"`:
```html
<a href="https://www.link.com" target="_blank">Linked Text to Display</a>
```

If you submit content that includes an image, make sure to include alt text in your link:
```html
<a href="https://www.imagelink.com"><img src="images/linkedimage.jpg" alt="Alternate text that describes the image"></a>
```

## Submit your changes

Here are the steps for submitting a change:

1. Create a pull request for the file you're updating.
2. Add a clear log message describing your changes.
3. Submit your pull request.

Please submit your changes with a [GitHub pull request](https://help.github.com/articles/about-pull-requests/) to [/OhioSuffrageCentennial/ohiosuffragecentennial]https://github.com/OhioSuffrageCentennial/ohiosuffragecentennial/pulls) with a clear list of the changes you're making. **Please, only one feature per commit.**

Include a clear log message for your commits. One-line messages are fine for small changes, but bigger changes should look like this:

```git
$ git commit -m "Brief summary of your commit"
>
> A paragraph describing what you changed and the impact of your changes."
```
