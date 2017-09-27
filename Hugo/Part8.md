# Part 8
## Archetypes

Under  `archetypes\default.md`

```md
---
title: "{{ replace .TranslationBaseName "-" " " | title }}"
date: {{ .Date }}
draft: true
---
```

This is the default frontmatter.

### define frontmatter for specific directories

- under `archetypes\` create a new file called `dir1.md`
- duplicate from default.md but add

```
---
title: "{{ replace .TranslationBaseName "-" " " | title }}"
date: {{ .Date }}
draft: true
author: "Steve"
---
```

- create a new file
```
$ hugo new dir1/new.md   
```

It automatically sends it to `dir1/` directory with our new frontmatter


