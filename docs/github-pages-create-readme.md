# Create the main GitHub Pages README file in /docs/README.md 

The first thing needed is to create a file named specifically `README.md` capitalized exactly as shown, 
and if you're using GitHub Pages, you should put it in a directory named `/docs`. 
Sites like the one you're creating with GitHub Pages often accompany code for a software project and `/docs` is the logical location.

More important, Jekyll expects your text to be in that directory as well.

GitHub pages sites use directory structures. Each subdirectory with pages you want published must contain
a README.md file, which will be silently converted to `index.html` files.

* Under **Quick setup — if you’ve done this kind of thing before** it says
`Get started by creating a new file or uploading an existing file. We recommend every repository include a README, LICENSE, and .gitignore`. 
Choose the `creating a new file` link:

![Creating a new repository](./assets/github-quick-setup.png)

* Enter `docs/README.md` and you'll see how GitHub separates the path and filename
interactively, visually distinguishing each level of the directory
hierarchy:

![Each slash creates a new directory](./assets/github-enter-directory-slash-filename.png)

All GitHub Pages directories with files meant to appear in the website
must have a file named `README.md` in them.

