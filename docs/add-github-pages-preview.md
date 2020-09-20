# Your GitHub Pages URL and adding preview to your README.md

It can be a little confusing, but when you're using GitHub and viewing a Markdown page you're seeing a simple
preview of that page with a style sheet chosen by GitHub. The style sheet is part of a Jekyll theme named `minima`. Neither can be changed
using GitHub preview. To view the document using your custom CSS formatting requires viewing it in GitHub Pages. It will still be using the `minima` theme but your CSS overrides what's in the `minima` theme.

All you have to do to see your document with its final formatting is figure out the GitHub pages address. Here's an example link:

View in [Github Pages](https://tomcam.github.io/least-github-pages/) or directly on [Github](https://github.com/tomcam/least-github-pages/) 
* [Your GitHub Pages URL and adding preview to your README.md](add-github-pages-preview.md)

## Determining the name of your GitHub Pages site

Your first job is to make sure you know the full URL of your GitHub repo. You will then use most of that information
to build up a URL based on a separate URL named `github.io`, not `github.com`.

### Get the name of your GitHub repo

Recalling [Creating a GitHub repository for your projects](creating-github-repository.md#repo-url), your GitHub repository address is
always made up of these components:

```
https://github.com/
```

Followed by your GitHub username/account name, and a `/` slash. The creator of this repo has the GitHub username `tomcam`, for example.

```
https://github.com/tomcam/
```

Followed by the name of the repo.

So the name of this repository is https://github.com/tomcam/least-github-pages:

```
https://github.com/tomcam/least-github-pages
```

### Use the elements of your GitHub repo URL to derive your GitHub Pages URL

Taking the parts of your URL, create the GitHub pages URL for it this way:

* Start with `https://` followed your GitHub account name, and a period after that. For example, if your GitHub account name
happened to be `tomcam`:

```
https://tomcam.
```

* Follow it with `github.io` NOT `github.com`:

```
https://tomcam.github.io
```

* Follow it with a slash `/` and your repo name. For example, if your repo name were `least-github-pages`, the GitHub.io address would be:

```
https://tomcam.github.io/least-github-pages
```

It's handy to put a link like this near the top of the document so your audience can view either the
GitHub Pages version or the GitHub repo preview:

```
View in [Github Pages](https://tomcam.github.io/least-github-pages/) or directly on [Github](https://github.com/tomcam/least-github-pages/) 
* [Your GitHub Pages URL and adding preview to your README.md](add-github-pages-preview.md)
```

## It can take a few moments to generate the current GitHub Pages page and formatting

GitHub Pages doesn't generate your new website every time you make changes to a repo. It updates "lazily", meaning
that it won't generate the website until someone actually browses to the GitHub Pages URL. It can take up to a minute 
or two for your GitHub Pages site to be generated the first time it's viewed.
