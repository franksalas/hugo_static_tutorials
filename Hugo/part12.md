# Part 12
## List page template

Act as a template for list pages

### Create own custom list theme

- under `first_site\layouts` create a folder called `_default`
- under that, create a file called `list.html'

```html
<!DOCTYPE html>
<html>
<head>
    <title>Custom List view</title>
</head>
<body>
    some Text here!

</body>
</html>
```

Display content using  hugo variables

```html
<!DOCTYPE html>
<html>
<head>
    <title>Custom List view</title>
</head>
<body>
{{.Content}}

</body>
</html>
```

It shows the content on the `_index.md` if any

Show all of the pages by using a hugo function

```html
<body>
    {{.Content}}

    {{range .Pages }}
        {{.Title}}<br>
        
    {{end}}
    </body>
```

Create a list of pages that link.

```html
<body>
{{.Content}}
    {{range .Pages }}
        <ul>
            <li>
                <a href="{{.URL}}">{{.Title}} </a>
            </li>
        </ul>
{{end}}
</body>
```