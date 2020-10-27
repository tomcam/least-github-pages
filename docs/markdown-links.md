# Create Markdown links to other pages on your site 

Start with a simple `README.md`:

```markdown
# Welcome to to Example.com

We hope you love this tiny tiny site.

Need to [contact someone](./contact.md) on the team?
```

## Linking to Markdown documents in the same directory

Creating a link to a document in the current Markdown directory is easy:

```
Need to [contact someone](./contact.md)?

```

## Terminology and sample directory structure to illustrate these examples

Here is a typical GitHub Pages directory structure.

```
docs/
  ├── README.md
  ├── _config.yml
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
   ```


### Root directory

For the purposes of these illustrations, we'll call `/docs` the root directory. If you're used
to Git projects or directory structure you may be puzzled because you might think of `/` as root.
GitHub Pages prefers your documentation to start in `/docs` because typically the actual `/` root is reserved for code.

### Subdirectory

In the above illustration, `tutorial` is a subdirectory of `/docs`. So are the `assets` and `reference` directories.
You might think of them as child folders or child directories, which is fine. The normal terminology is
subdirectory, though.

Depending on context, you might see these directories called `/assets`, `/reference`, or `/tutorial`.
That's because the implied root directory is `/docs`. Their full designations would be `/docs/assets` and so forth.

The `v1` directory is a subdirectory of `/reference`, so it is likely to be referred to in these documents as
`/reference/v1` even though it's technically `/docs/reference/v1`

### Parent directory

The opposite of a subdirectory is a parent directory. So:

* `/` is the parent of the `docs` directory
* `/docs` is the parent of the `reference` directory
* `/docs/reference` is the parent of the `/v1` directory

### Path

Any description of a file location is called a path. 
For example, the full pathname of `README.md` in the above example is `/docs/README.md`. 
The correct term for that path is either *absolute path* or *fully qualified pathname*, for the most part it's just called the path in this guide.

### Relative directories

The last couple of points describe relative directories. Relative directories also have notation, where a single dot followed by a slash `./` refers to the current directory, and two docs followed by a slash `../` refer to the parent directory. So:

* A link from within the document `contact.md` to the file `screenshot-home-1024x512.png` would look like this: `assets/img/screenshot-home-1024x512.png` (no relative notation used)
* A relative link from within the document `start.md` to the file `chapter1.md` would be notated as `../chapter1.md` in relative terms.
* A link from within the document `start.md`  to the file `contact.md` could be notated as *without* a relative path as `/docs/contact.md`,
which is also termed a *fully qualified pathname*.
* A link from within the document `reference1.0.md` to `chapter1.md` would be notated as`../../chapter1.md` in relative terms.

## Linking to Markdown documents in a subdirectory/child directory

Building on [relative directories](#relative-directories), here are full examples.
                                                    

## GitHub-flavored Markdown links with .md get silently converted to HTML links

If you're used to HTML, you're probably noticing something on odd. 
The link goes to `contact.md`, not `contact.html`, and we know the
job of a static site generator like Jekyll, which is used by GitHub,
is to convert Markdown files to HTML. How does this turn into a valid link?

Jekyll sees internal links like `contact.md` and converts
them to something like `contact` or `contact.html`. The GitHub webserver observes this convention too.

### GitHub-flavored Markdown differs from standard [Markdown](https://commonmark.org)

GitHub uses an extended version of Markdown.
The internal linking feature is one element of many. For complete details, see the
[GitHub-flavored Markdown Spec](https://github.github.com/gfm/) technical spec.


A link from within `README.md` to `article 2.md` would therefore look like this:

```markdown
Take a look at [Article 2](/chapter3/article2.md) for more information.
```

[Back](/README.md)

