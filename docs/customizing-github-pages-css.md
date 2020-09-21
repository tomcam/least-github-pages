# Adding an assets directory to your GitHub Pages site

While you can store any kind of file in a GitHub directory, certain files get better treatment than others.
If you want image files in your repo to display, or to customize the CSS, the easiest way is to follow 
Jekyll conventions and create an [assets directory](https://jekyllrb.com/docs/step-by-step/07-assets/).
Here's how to do it in GitHub Pages. The assets directory should contain subdirectories for CSS and images.

## Assets

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

* After typing the filename go down to the editor and give it these contents:

```
---
---
@import "{{ site.theme }}";
```

* Choose the green **Commit new file** button to save your work.

You've just created a minimal SASS file.

## CSS

CSS, or Cascading Style sheets, lets you create a master file that changes the appearance of all
HTML files that include it. For example, suppose you want all level 2 headers to be colored red.
You can do that by adding a 12 characters CSS rule, as illustrated below.

### Jekyll, CSS, SASS, and SCSS files

Since CSS is a bit limited regarding variables, namespace scoping, and expression evaluation, Jekyll uses
a preprocessor named [SASS](https://sass-lang.com/guide) as its default style sheet formatting system.
SASS files end in `.scss`, and by tradition the main such file is named `style.scss`. Part of the build
process of converting a Jekyll site to the published HTML is reading the `.scss` file, then translating it into CSS. 

Use of SASS is out of the scope of this document, but luckily SASS lets you use plain CSS so we'll just
use CSS in the `style.scss` file in the examples here. All you need to do is put your CSS after the `@import "";` line.

### Testing a CSS addition

Let's try a harmless change to your CSS to illustrate its behavior on GitHub Pages.

* Choose the `/docs/assets/css/style.scss` link to the file you just created, then click the Pencil icon so you can edit it.

You should see this:

```
---
---
@import "{{ site.theme }}";
```

* Add `h2 {color:red}` under the `@import statement`, like this:

```
---
---
@import "{{ site.theme }}";

h2 {color:red}
```
* Choose the green **Commit new file** button to save your work.

