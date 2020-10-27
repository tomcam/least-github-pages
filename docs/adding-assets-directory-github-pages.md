# Adding an assets directory to GitHub Pages 

GitHub Pages is based on [Jekyll](https://jekyllrb.com), which expects graphic images and custom CSS to be
in a directory named `assets`.

While you can store any kind of file in a GitHub directory, certain files get better treatment than others.
If you want image files in your repo to display, or to customize the CSS, the easiest way is to follow 
Jekyll conventions and create an [assets directory](https://jekyllrb.com/docs/step-by-step/07-assets/).
Here's how to do it in GitHub Pages. The assets directory should contain subdirectories for CSS and images.

## Create the directory /docs/assets/css

Creating an assets directory is a two-step process because Git doesn't recognize empty directories.
You will therefore need to create the assets directory and add at least an empty style sheet (or any other file)
at the same time.

Jekyll prefers the `assets` directory  is directly under the `/docs` directory. So:

* From the root of your repository, choose the `docs` folder.

* Click the **Add file** button, then choose **Create new file**.

* For the file name, enter `assets/css/style.scss`, meaning its full representation will be  `your-username/your-repo/docs/assets/css/style.scss`, where `your-username` is your GitHub username and `your-repo` is the name of the repository
you just created.

Notice that each type you type a slash, the GitHub editor creates a new subdirectory. That's 
just what you want to happen.

### Creating the style.scss file

Now it's time to add text to the empty file.

* After typing the filename go down to the editor and give it these contents, where `site.theme` is literally
what you'd type below.

```
---
---
@import "{{ site.theme }}";
```

* Choose the green **Commit new file** button to save your work.

You've just created a minimal SASS file.

### Jekyll, CSS, SASS, and SCSS files

CSS is a bit limited regarding variables, namespace scoping, and expression evaluation. Jekyll uses
a preprocessor named [SASS](https://sass-lang.com/guide) as its default style sheet formatting system.
SASS files end in `.scss`, and by tradition the main such file is named `style.scss`. Part of the build
process of converting a Jekyll site to the published HTML is reading the `.scss` file, then translating it into CSS. 

## Image files

You can put image files anywhere in the `assets` directory. Jekyll prefers them in `assets/images` but this publication simply puts them in `assets` itself.

[Back](/README.md)

