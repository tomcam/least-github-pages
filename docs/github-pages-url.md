# Determining your GitHub Pages URL

It can be a little confusing, but when you're using GitHub and viewing a Markdown page you're seeing a simple
HTML rendering of that page with a fixed style sheet chosen by GitHub.  You need a different link
to view it in GitHub Pages using one of the GitHub Pages Jekyll themes.

All you have to do to see your document with its final formatting is figure out the GitHub Pages address. 
Here's the Markdown source to both links:

```markdown
View on [Github Pages](https://tomcam.github.io/least-github-pages/)
```

```markdown
View on [Github](https://github.com/tomcam/least-github-pages/)
```

Here's how to create the GitHub Pages URL from the GitHub URL.

## Get the full URL of your GitHub repo

Your first job is to make sure you know the full URL of your GitHub repo. 
For example, the name of this repository is `https://github.com/tomcam/least-github-pages`. Here's how it breaks down.

### Start with the GitHub URL

Recalling [Creating a GitHub repository for your projects](creating-github-repository.md#repo-url), your GitHub repository address is
always made up of these components:

The GitHub website URL:

```
https://github.com/
```

### Add the username and a slash

Followed by your GitHub username/account name, and a `/` slash. The creator of this repo has the GitHub username `tomcam`, for example.

```
https://github.com/tomcam/
```

### Add the name of your GitHub repo


Followed by the name of the repo, so:

```
https://github.com/tomcam/least-github-pages
```

## The GitHub Pages repository URL is always https://{userid}.github.io/{reponame}

The GitHub Pages URL is based on the GitHub repo URL, and takes the format `https://{userid}.github.io/{reponame}`.
The moment you use it, GitHub Pages will generate a website based on the contents of your repo.


### Use the elements of your GitHub repo URL to derive your GitHub Pages URL

Taking the parts of your URL, create the GitHub pages URL for it this way:

### Start with https:// and your username

* Start with `https://` followed your GitHub account name, and a period after that. For example, if your GitHub account name
happened to be `tomcam`:

```
https://tomcam.
```
### Add github.io

* Follow it with `github.io`, **not** `github.com`:

```
https://tomcam.github.io
```

### Add slash and the repo name

* Follow it with a slash `/` and your repo name. For example, if your repo name were `least-github-pages`, the GitHub.io address would be:

```
https://tomcam.github.io/least-github-pages
```

### Example

So this GitHub URL:
```markdown
[Github](https://github.com/tomcam/least-github-pages/)
```

Becomes:
```markdown
[Github Pages](https://tomcam.github.io/least-github-pages/)
```

Note that the parts in square brackets, `[GitHub]` in the first example, and `[GitHub Pages]`, can be any text. They
form the clickable link in the final rendered HTML.



