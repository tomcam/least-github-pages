# Creating a GitHub Account

You only need to do this once:

* First [Join GitHub](https://github.com/join). It's free.

Your GitHub account is allowed unlimited public projects.
This guide shows how to create a GitHub Pages site from a public project.

## Creating a repository for your projects

* Choose the **+** menu, then **New repository**.

The **Create a new repository** page appears.

![Creating a new repository](./assets/create-new-github-repository.png)

* Give it a name made up of lowercase letters, numbers, and hypen characters (the minus sign, or `-`) instead
of spaces. It will be used as a filename, and it will be given prominence in Web searches.

* Leave **Public** checked, then choose **Create repository**

You're not done yet!

## Creating a gh-pages branch

Since websites like the one you're creating with GitHub Pages often accompany
something like the code for a software project, GitHub Pages has a shortcut.
It treats a branch named `gh-pages` specially, shortening some of the
steps to publishing. Let's create a branch by that name.

You'll see a button that says **Branch: master**.

* Click the  **Branch: master** button

A **Switch branches/tags** dropdown appears.

* Enter **gh-pages** into the textbox.

* When you're finished, click the area below that says **Create branch: gh-pages**.

![Creating a branch named gh-pages](./assets/github-create-gh-pages-branch)

The button should now say **Branch: gh-pages**.

## Creating a /pages directory with a README.md file in it

A Quick setup page appears. You'll see a message that says `Get started by creating a new file or uploading an existing file.`

The source code for your site must be in a directory called `/pages` but there's no way to
create a directory without a file in GitHub. You must enter a filename but precede it
with a directory name (`pages`) in this case. The directory name will get created
automatically.

Luckily you need a file. All GitHub Pages directory with files meant to appear in the website
must have a file named `README.md` in them.

* Click `creating a new file`.

![The create a new file page](./assets/quick-setup-create-a-new-file.png)

* Start typing the directory name, `pages`:

![](./assets/create-a-new-file-pages-directory.png)

Here's where the directory gets created.

* Type a slash character (`/`), then the name of the file, `README.md` in this case:

![Creating a pages directory and a README.md file at the same time](./assets/github-create-readme-file.png)

* You've now created a file named README.md in the `/pages` directory of the repo.

* Add a line starting with the pound sign/hash tag. It's a title that will be converted
to an HTML `<h1`> tag, so something like `# Foobar tutorial`. Then add a blank line, followed by some 
text, say, `Thanks for using Foobar`. Here's what it will look like:

![Editing the README.md file](./assets/github-pages-edit-readme.png)

When you're finished, click **Commit changes** at the bottom of the page. 
Normally you'd put a comment there, but the default (`Create README.md`) does the job
just fine.

![Saving the README.md file](./assets/github-pages-save-readme.png)

After it's saved you see a preview:

![README.md file in preview mode](./assets/github-preview-readme.png)

If you wanted you could edit the file again by choosing the pencil icon.

