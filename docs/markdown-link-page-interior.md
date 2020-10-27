### Link to headers inside a file 

GitHub Pages secretly turns every header into its own named file location.
This lets you navigate not just to a file, but to any header
in that file. You do it by following the filename with the header,
where spaces have been removed and punctuation is replaced with
spaces. For example, `contact.md#rosie-greer`. Here's a 
complete illustration.

Take the following file named `contact.md`:

```markdown
# Contact

Here's whom to call when you have a problem.

## Tyler Perry

He has two first names! How cool is that?

## Rosie Greer

When two heads are better than one.
```

Suppose you want to link right to Rosie, not just to the Contact page itself?

Let's try linking to Rosie's location inside `contact.md` in a slightly modified `README.md`:

```markdown
# Welcome to to Example.com

## This just in!

Good news! [Rosie's](./contact.md#rosie-greer)
head graft is a major success!

Let's face it. You're darn lucky to be here.

Need to [contact someone](./contact.md) on the team?
```

As you can see, the anchor to a header such as `## Rosie Greer` flattened out. 
Everything gets converted to lower case, and spaces are replaced with hypens.
This location name is synthesized as `#rosie-greer`:

```
Good news! [Rosie's](./contact.md#rosie-greer)
head graft is a major success!
```

If you click Rosie's name you'll
be taken directly to that position in the file.

[Back](/README.md)

