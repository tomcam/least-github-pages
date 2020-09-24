# Creating Markdown links to other pages on your site 

Start with a simple `README.md`:

```markdown
# Welcome to to Example.com

We hope you love this tiny tiny site.

Need to [contact someone](./contact.md) on the team?
```

## GitHub-flavored Markdown links with .md get silently converted to HTML links

If you're used to HTML, you're probably noticing something on odd. 
The link goes to `contact.md`, not `contact.html`, and we know the
job of a static site generator like Jekyll, which is used by GitHub,
is to convert Markdown files to HTML. How does this turn into a valid link?

By a modest level of trickery.  Jekyll, along with the way GitHub Page's
webserver is tuned, sees internal links like `contact.md` and converts
them to something like `contact` or `contact.html`.

### GitHub-flavored Markdown differs from standard [Markdown](https://commonmark.org)

GitHub wanted extra features of Markdown, so it add many features to the specification.
The internal linking feature is one element of many. For complete details, see the
[GitHub-flavored Markdown Spec](https://github.github.com/gfm/) technical spec.

## Page hierarchies using folders

The simplest layout for a GitHub Pages repository looks something like this.

```markdown
docs/
  ├── README.md
  ├── about.md
  ├── contact.md
  ├── chapter1.md
  ├── chapter2.md
  └── tutorial/
        ├── start.md
        └── config.md

docs/
  ├── README.md
  ├── about.md
  ├── contact.md
  ├── chapter1.md
  ├── chapter2.md
  ├── assets/
  │     ├── css/
  │     │    └── style.scss
  │     └── img/
  │          └── screenshot-home-1024x512.png
  ├── tutorial/
  │     ├── start.md
  │     └── config.md
  └── reference/
        ├── v1/
        │    └── reference1.0.md
        └── v2/
             └── reference2.0.md




/do cs └── 
┌── README.md
├── about.md
├── contact.md
├── chapter1.md
└── chapter2.md
```

If you have sections consisting of more than one file, it's very 
useful to put them in subdirectories. Each subdirectory must
contain a `README.md` of its own. 
 
```
┌── README.md
├── chapter1.md
├── chapter2.md
└── chapter3/
        ├── article1.md
        └── article2.md
```

A link from within `README.md` to `article 2.md` would therefore look like this:

```markdown
Take a look at [Article 2](/chapter3/article2.md) for more information.
```
