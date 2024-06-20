---
tags:
  - Seedling
  - Inbox/Books
created: 2024-06-20T22:18
updated: 2024-06-20T22:19
---

up::
```dataviewjs
// Get the current file's name
const currentFileName = dv.current().file.name;

// Extract the book title from the chapter's name
const bookTitle = currentFileName.split(' - ')[0].replace(/^\{\{\s*/, '');

// Create a regular expression to match the book and all its chapters
let regex = new RegExp(`^\\{\\{? ${bookTitle.replace(/[-\/\\^$*+?.()|[\]{}]/g, '\\$&')}( - Chapter \\d+)?$`, 'i');

// Query and display the book and chapters
dv.pages()
  .where(page => regex.test(page.file.name))
  .sort(p => p.file.name, 'asc')
  .forEach(page => {
      dv.paragraph(`- [[${page.file.link.path}|${page.file.name}]]`);
  });

```

# <% tp.file.cursor(0) %>

## Takeaways

- 

## What I learned (In My Own Words)

- 
