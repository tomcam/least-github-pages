# The Least You Need to Know About GitHub Pages

This guide shows you how to create information-heavy websites quickly 
and interactively using GitHub Pages right on the GitHub website. You
don't need to learn command-line programs like Git or install anything
on your own computer.

GitHub Pages is free if your repository (file storage area) is public.

**Ways to view this site**
* [Github Pages](https://tomcam.github.io/least-github-pages/)
* Directly on [Github](https://github.com/tomcam/least-github-pages/) 

If you were pointed here by an employer or well-meaning friend and aren't quite sure why, 
plenty of reasons this guide may help you are in [Why Use GitHub Pages?](why-use-github-pages.md)

**What this guide is for:** This guide is laser-focused on one thing: showing how to get a working informational website up and running as fast
as possible using GitHub Pages, using only the GitHub website. *Informational website* is an informal term meaning that the emphasis is on
function (structured text with simple formatting, links, images) and not form (intricate page design). It goes step by step from the very beginning
and assumes very little knowledge on your part.

**What you can get out of this guide:**  If you follow through the steps in this guide you'll have a small website demonstrating everything you need to put up an attractive, easy to maintain site using words, links, and images. 
You'll do this all on the free GitHub website, without having to download or install anything.
Not covered are advanced topics such as using Git on the command line, custom themes, SEO, version control,
and advanced features of GitHub-flavored Markdown.

## Table of contents

This short GitHub Pages tutorial discusses:

* [Intended audience](#intended-audience)
* [Create a GitHub Account](creating-github-account.md)
* [Create a GitHub repository](creating-github-repository.md)
* [Enable GitHub Pages](enable-github-pages.md) so you can create and publish a formatted website 
* [Set the GitHub Pages master branch to the /docs folder](set-github-pages-master-branch.md)
* [Create the main GitHub Pages README file in /docs/README.md](github-pages-create-readme.md)
* [Create a web page on GitHub](create-page-github.md) using Markdown
* [GitHub Pages directory and file usage](github-pages-directory-file-usage.md)
* [Creating Markdown links to other pages on your own site](markdown-links.md)
* [Headers in Markdown](markdown-headers.md)
* [Creating Markdown links to other sites](markdown-links-to-other-sites.md)
* [Creating Markdown links to the interior of a page](markdown-link-page-interior.md)
* [Adding an assets directory to your GitHub Pages site](customizing-github-pages-css.md#assets)
* [Adding Custom CSS to GitHub Pages](customizing-github-pages-css.md##css)
* [TODO: Publish your pages as a GitHub Pages website](publish-to-github-pages.md)
* [Your GitHub Pages URL and adding preview to your README.md](add-github-pages-preview.md)
* [TODO: Add images to your GitHub Pages site](adding-images-github-pages-site.md)
* Change the appearance of your site using Jekyll themes

## Intended audience

GitHub Pages uses [Jekyll](https://jekyllrb.com), a publishing system based on the Ruby programming language. The Jekyll documentation is excellent, especially if you already know Jekyll, program in Ruby, and have both Ruby and Jekyll installed on your local computer. The GitHub Pages documentation is comprehensive and excellent--if you're already a Jekyll expert.

[The Least You Need to Know About GitHub Pages](./) is designed for people who don't happen to know Jekyll already but who need to get up to speed in GitHub Pages quickly to get a job done *now*. It tells you not only what to do step by step,
but also briefly explains why you take each step.

You probably don't want to use this guide to create web pages that require complex, individual formatting on a per-page basis. 
GitHub Pages uses Markdown, which has some limited formatting information but not a lot.
GitHub Pages then uses Jekyll to turn that Markdown into HTML, based on the Jekyll theme you've chosen. Generally speaking this approach is
absolutely ideal for blogs, technical documents and instructional materials that require versioning and collaboration, where the
main work product is words and pictures. It is not a good fit for things like boutique pages, restaurant menu sites, consumer product sites, and so on where
custom formatting is the norm. 

### Advantages to using GitHub Pages

Still wondering whether to use GitHub Pages? See [Advantages to using GitHub Pages to generate static sites](github-pages-advantages.md)

### Disadvantages to using GitHub Pages

If you want to understand why GitHub pages may not suit your project, see [When to avoid GitHub pages](github-pages-disadvantages.md).

