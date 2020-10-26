# Determining your GitHub Pages URL

It can be a little confusing, but when you're using GitHub and viewing a Markdown page you're seeing a simple
preview of that page with a style sheet chosen by GitHub. The style sheet is part of a Jekyll theme named `minima`. Neither can be changed
using GitHub preview. To view the document using your custom CSS formatting requires viewing it in GitHub Pages. It will still be using the `minima` theme but your CSS overrides what's in the `minima` theme.

All you have to do to see your document with its final formatting is figure out the GitHub pages address. 
Here's the Markdown source to an example link:

```markdown
[Github Pages](https://tomcam.github.io/least-github-pages/) or [Github](https://github.com/tomcam/least-github-pages/) 
```

Here is the actual link:

See in [Github Pages](https://tomcam.github.io/least-github-pages/) or on [Github](https://github.com/tomcam/least-github-pages/) 

## Get the full URL of your GitHub repo

Your first job is to make sure you know the full URL of your GitHub repo. 
For example, the name of this repository is `https://github.com/tomcam/least-github-pages`. Here's how it breaks down.

### Get the name of your GitHub repo

Recalling [Creating a GitHub repository for your projects](creating-github-repository.md#repo-url), your GitHub repository address is
always made up of these components:

The GitHub website URL:

```
https://github.com/
```

Followed by your GitHub username/account name, and a `/` slash. The creator of this repo has the GitHub username `tomcam`, for example.

```
https://github.com/tomcam/
```

Followed by the name of the repo, so:

```
https://github.com/tomcam/least-github-pages
```

## The GitHub Pages repository URL is always https://{userid}.github.io/{reponame}

The GitHub Pages URL is based on the GitHub repo URL, and takes the format `https://{userid}.github.io/{reponame}`.
The moment you use it, GitHub Pages will generate a website based on the contents of your repo.


### Use the elements of your GitHub repo URL to derive your GitHub Pages URL

Taking the parts of your URL, create the GitHub pages URL for it this way:

* Start with `https://` followed your GitHub account name, and a period after that. For example, if your GitHub account name
happened to be `tomcam`:

```
https://tomcam.
```

* Follow it with `github.io`, **not** `github.com`:

```
https://tomcam.github.io
```

* Follow it with a slash `/` and your repo name. For example, if your repo name were `least-github-pages`, the GitHub.io address would be:

```
https://tomcam.github.io/least-github-pages
```
