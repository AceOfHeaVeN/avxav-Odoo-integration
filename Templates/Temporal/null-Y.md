---
tags: 
aliases: 
created: 2024-06-20T22:18
updated: 2024-06-20T22:19
---

# Annual Review:

[[-1-Y]] <== <button class='date_button_today'>This Year</button> ==> [[NaN-Y]]

## Aliases

```dataview
TABLE aliases
FROM "Journal"
WHERE aliases != null
WHERE length(aliases) > 1
WHERE file.day.year = null
```

## Highlights

```dataview
TABLE WITHOUT ID dateformat(file.ctime, "yyyy-MM") AS Month, file.day.weekyear AS Week, highlights
FROM "Journal"
WHERE highlights != null
WHERE file.day.year = null
SORT file.day.weekyear
```

