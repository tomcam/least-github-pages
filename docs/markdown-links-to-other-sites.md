## Create Markdown links to other sites

Let's review what happens to links in Markdown files.

Markdown such as `[contact someone](./contact.md)` gets turned into an HTML link to
a page in your repository. The part 
of the link in square brackets, `contact someone` in this case, becomes the anchor text (the
visible part of a link, and the part that gets indexed by search engines). The part in 
parentheses, `./contact.md` in this case, becomes a reference to an HTML file by the same 
name, which would be `contact.html` in the current directory.

### Linking to external web sites using Markdown

The format for linking to other websites is similar to Markdown but you just
use the website's actual URL in parentheses. For example:

```markdown
Try [Google](https://www.google.com/) for more info.
```

[Previous page](markdown-headers.md)  | [Next page](markdown-link-page-interior.md)

#### [Home](/README.md) 
