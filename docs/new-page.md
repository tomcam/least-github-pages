# Create a new page and link to it

Let's see how linking works by creating a second page, then linking to it from the first.

## Add a new page to the /docs directory

* Navigate back to your project directory by clicking the project name at the upper left of the page.

* Choose the `/doc` directory link. This is important because you don't want your
files to end up in the root directory.

* Choose **Create new file** and give it the name `tutorial.md`:

![Create a file named tutorial.md in the /docs directory](./assets/github-create-tutorial-md-file.png)

* Give it these contents:

```md
# Quick start tutorial

Here's how to get up and running as fast as possible.
We'll explain the details later.
```

* Move to the bottom of the page and choose **Commit changes** to save this file.

GitHub shows you the contents of the `/docs` directory. It should appear alongside README.md:

![tutorial.md file next to README.md in GitHub](./assets/tutorial-and-readme.png)


## Edit the original README.md and link to the new tutorial page

* Navigate back to your project directory by clicking the project name at the upper left of the page.

* Choose the `/doc` directory link, then choose `README.md`.

It appears rendered in HTML. 

![README.md preview](./assets/github-pages-nav-tutorial.png)


* Click the pencil icon to edit it 
and add the following line:


```md{3}
# Please start here

Thanks for using our product.

If you want to dive right in, 
try our [quick start tutorial](tutorial.md). 
```

* Choose **Commit changes** to save.;

The HTML preview of the new `README.md` appears with 
the text you added rendered as a link:

![Link added to README.md](./assets/github-pages-link-added.png)

* Click the link and you'll navigate to GitHub's preview of the tutorial page:

![Tutorial page preview](./assets/github-pages-tutorial-md.png)


