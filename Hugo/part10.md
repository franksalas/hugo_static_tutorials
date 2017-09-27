# Part 10
## Taxonomies

How we group content together.

Hugo provides by default two taxonomies.

- tags
- categories


### Add tags & categories to our files

add `tags:`  and `categories: ` to our frontmatter file

```frontmatter
---
title: "a"
date: 2017-01-26T19:42:38-05:00
draft: true
author: "frank"

tags: ["tag1", "tag2", "tag3"]
categories: ["cat1"]
---
```

Hugo creates `http://localhost:1313/tags/mytags` and `http://localhost:1313/categories/my_categores/` for every tag and categorie created.

## create custom taxonomies

- Add a new taxonomy called `moods:` on our md file

```frontmatter
...
tags: ["tag1", "tag2", "tag3"]
categories: ["cat1"]
moods:["happy", "crazy"]
---
```

- go to the `config.toml` file and add it 

```toml
.
...
theme = 'ga-hugo-theme'


[taxonomies]
    tag = "tags"
    category = "categories"
    mood = "moods"

```

