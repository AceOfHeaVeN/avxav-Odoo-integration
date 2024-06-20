---
read_book: 
good_reads_review: 
roth_ira: 
youtube_collab: 
ulfar_event: 
social_outing: 
created: 2024-01-11T02:26
updated: 2024-06-20T22:19
---

# Monthly Review:
%% This template Requires the Templater plugin %%
[[2024-M05]] <== <button class="date_button_today">This Month</button> ==> [[2024-M07]]

---

```dataview
TABLE aliases
FROM "2 Journal"
WHERE aliases != null
AND file.day.year = number(substring(this.file.name, 0, 4))
AND dateformat(date(file.name), "yyyy-MM") = replace(this.file.name, "M", "")
SORT file.day
```

---

```dataview
TABLE WITHOUT ID file.day.weekyear AS Week, highlights
FROM "2 Journal/Daily"
WHERE highlights != null
AND file.day.year = number(substring(this.file.name, 0, 4))
AND dateformat(date(file.name), "yyyy-MM") = replace(this.file.name, "M", "")
SORT file.day
```






---






```dataview
TABLE WITHOUT ID file.day.weekyear AS Week, meditations
FROM "2 Journal/Daily"
WHERE meditations != null
AND file.day.year = number(substring(this.file.name, 0, 4))
AND dateformat(date(file.name), "yyyy-MM") = replace(this.file.name, "M", "")
SORT file.day
```






---






```dataview
TABLE WITHOUT ID file.day.weekyear AS Week, foods
FROM "2 Journal/Daily"
WHERE foods != null
AND file.day.year = number(substring(this.file.name, 0, 4))
AND dateformat(date(file.name), "yyyy-MM") = replace(this.file.name, "M", "")
SORT file.day
```