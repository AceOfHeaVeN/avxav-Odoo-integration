---
tags: 
read_book?: 
exercised?: 
meditated?: 
typingSpeed: 
mood: 
aliases: 
created: 2023-12-15T18:02
updated: 2024-02-04T16:52
---

> [!todoist]- Todoist - Overdue
> ```todoist  
> name: My Tasks  
> filter: overdue
> sorting:  
> - date  
> - priority  
> group: true
> ```

> [!todoist]- Todoist - Today
> ```todoist  
> name: My Tasks  
> filter: today
> sorting:  
> - date  
> - priority  
> group: true
> ```

## On This Day...

If you created a note last year (or any other different year) on this exact date and day, and you want to see what it contained, you will find it here:

```dataview
LIST 
FROM "2 Journal/Daily"
WHERE dateformat(file.day, "MM-dd") = dateformat(this.file.day, "MM-dd")
AND file.day != this.file.day
```

---

## Notes Created Today

```dataview
TABLE created, updated as modified, tags, type, status
FROM "" AND !"2 Journal" AND !"5 Extra/Templates"
WHERE contains(dateformat(file.ctime, "yyyy-MM-dd"), dateformat(this.file.day, "yyyy-MM-dd"))
```

---

## Highlights For Today

```dataview
TABLE highlights
FROM "2 Journal/Daily"
WHERE this.file.name = file.name
AND highlights != null
```

---

[[<% tp.date.now("YYYY-MM-DD", -1, tp.file.title, "YYYY-MM-DD") %>]] <== <button class="date_button_today">Today</button> ==> [[<% tp.date.now("YYYY-MM-DD", 1, tp.file.title, "YYYY-MM-DD") %>]]

## Zaid, Add Your Daily Variables Here 

---

<% tp.file.cursor(0) %>

## So, What's On Your Mind Today? 

---

<%* if (tp.date.now("M-D") == "1-1") { %>
**Make Yearly Note**
<%* } _%>
<%* if (tp.date.now("D") == 1) { %>
**Make Monthly Note**
<%* } _%>
<%* if (tp.date.now("ddd") == "Sun") { %>
**Make Weekly Note**
<%* } _%>
<% tp.file.cursor(1) %>