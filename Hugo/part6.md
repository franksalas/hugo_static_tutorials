# Part 6
## Createing & Organizing Content

To crate a new file under `content/`
- `hugo new a.md`

### inside md file
- front matter: metadata of file,

### Create a file inside another directory

```bash
hugo new dir1/b.md
```

### run server w/ drafts
```bash
hugo server -D
```

Go to ` http://localhost:1313/`

The url reflects the location inside of the file inside the content folder
- http://localhost:1313/dir1/b/:  `content/dir1/b.md`
- http://localhost:1313/a/ : `content/a.md`

##  Two types of contents

### List Pages
- Homepage
- Content that list other content

### Single pages
- single content
- a page `.md` that list content.

## Create multiple single pages
directory:
```bash
contents\
    dir1\
        dir2\
            d.md
        b.md
        c.md
    dir3\
        e.md
        f.md
```

## Create list page manually
Hugo does not create a list page automatically for dir inside other dir on content.

- create an index.md file
```$
hugo new dir1/dir2/_index.md
```

## Overwrite pages that are created automatically
####  Add content



