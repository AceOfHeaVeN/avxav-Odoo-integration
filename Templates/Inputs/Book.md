---
tags: 
aliases: 
authors: 
general_subject: 
specific_subject: 
publish_date: 
created: 2024-06-20T22:18
updated: 2024-06-20T22:19
---

```dataviewjs
// Get the current file's name
const currentFileName = dv.current().file.name;

// Assume the current file is a book; remove the initial '{ ' from the name
const bookTitle = currentFileName.replace(/^\{\s*/, '');

// Create a regular expression to match the book and its chapters
let regex = new RegExp(`^\\{\\{ ${bookTitle.replace(/[-\/\\^$*+?.()|[\]{}]/g, '\\$&')} - Chapter \\d+$`, 'i');

// Query and display the chapters
dv.pages()
  .where(page => regex.test(page.file.name))
  .sort(p => p.file.name, 'asc')
  .forEach(page => {
      dv.paragraph(`- [[${page.file.link.path}|${page.file.name}]]`);
  });

```

## Notes:

```dataview
TABLE bookhighlights as SUMMARY
FROM [[]]
WHERE bookhighlights
SORT file.ctime ASC
```

> [!context]
> %%(How this article relates to other work in the field; how it ties in with key issues and findings by others, including yourself)%%
> - 

> [!significance]
> %%(to the field; in relation to your own work)%%
> - 

## Other Comments (Add Your Notes Here):

- 
