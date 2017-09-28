# Part 13
## Single page template

Use single tempaltes

### overide our theme template

- Create a folder under `layouts/` called `_default`.
- inside create a doc called `single.html`

From now on this is the default single page file, Hugo will ignore the original from theme.


How do we get the content from md files?
```html
<!DOCTYPE html>
<html>
<head>
    <title>single page</title>
</head>
<body>
    {{.Content}}

</body>
</html>
```
`{{.Content}}`  grabs the content from markdown file.

We can also use the frontmatter variabels.


```html
<!DOCTYPE html>
<html>
<head>
    <title>single page</title>
</head>
<body>
    <h3>This is title: {{.Title}}</h3>
<h4>This is date: {{.Date}}</h4>
    <p>This is content: {{.Content}}</p>
</body>
</html>
```

- `{{{.Title}}}`  gets the `title:` from the frontmatter variable.
- `{{.Date}}` gets the `date:` from the frontmatter variable.


