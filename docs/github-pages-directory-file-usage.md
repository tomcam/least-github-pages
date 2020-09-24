# GitHub Pages directory and file usage, from minimal to typical

Here are illustrations of what a GitHub pages repositories looks like, from
the bare minimum to what you will likely do on most projects.

## Minimum GitHub Pages repository with default appearance

The absolute minimum GitHub Pages repository for our purposes looks something like this.

```
docs/
  └── README.md
```

**Result:** When viewed on GitHub Pages, this would render pages using the default GitHub Pages Jekyll theme.

## Slightly more complex GitHub pages repository with default appearance

If you have sections consisting of more than one file, it's very 
useful to put them in subdirectories when the organization suggests it.

This repo is more like what a simple information site would be 
structured. It has a single subdirectory named `tutorial` in which a set of
related files resides.

**Result:** When viewed on GitHub Pages, this would render pages using the default GitHub Pages Jekyll theme.
It would contain links inside the directory hierarchy.

```
docs/
  ├── README.md
  ├── about.md
  ├── contact.md
  ├── chapter1.md
  ├── chapter2.md
  └── tutorial/
        ├── start.md
        └── config.md
```

## Minimum "standard" GitHub Pages repository with theme and custom stylesheet support

* To use something other than the default GitHub Pages theme, GitHub's Jekyll requires that you put the name of the theme
in a file named `_config.yml` placed in the root of your GitHub Pages repository. 
* To customize the CSS in the current theme,  GitHub's Jekyll requires that you need to put that CSS in a file named `style.scss` 
placed in a directory named `docs/assets` as shown below.
* By convention it's good to put image files in the `/assets` directory, typically in a subdirectory named `img`.

```
docs/
  ├── README.md
  ├── _config.yml
  └── assets/
       ├── css/
       │    └── style.scss
       └── img/
            └── screenshot-home-1024x512.png
```

**Result:** When viewed on GitHub Pages, this would render pages using whatever GitHub Pages Jekyll theme you specified in 
`_config.yml`.

## Typical GitHub Pages repository with theme and custom stylesheet support

Here's a fleshed-out example of a GitHub Pages repository with full theme and customized CSS support.
It's no different than the previous example other than showing a slightly more realistic file and
directory layout.

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
**Result:** When viewed on GitHub Pages, this would render pages using whatever GitHub Pages Jekyll theme you specified in 
`_config.yml`. It would contain links inside the directory hierarchy.
