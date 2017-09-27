# Part 11
## Template Basics

A hugo theme is made of several templates

## overview of templates

- go to  themes/ga-hugo-theme/layouts

- under layouts go to `_default`
- the `list.html` is the skeleton of our main page.

Example: `list.html`
```html

<body>
     {{ partial "header" (dict "Kind" .Kind "Template" "List") }}
     {{.Content}}
     {{ range .Pages }}

...
```
The `{{.Content}}` section of the file is where the content is injected.


