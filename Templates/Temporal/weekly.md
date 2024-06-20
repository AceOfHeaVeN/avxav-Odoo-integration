
# Weekly Review:


%% This template Requires the Templatr plugin and should be run on sundays, if not on sundays, the value offsets should be adjusted %%

[[<% tp.date.now("gggg-[W]ww", -1, tp.file.title, "gggg-[W]ww") %>]] <== This Week ==> [[<% tp.date.now("gggg-[W]ww", +7, tp.file.title, "gggg-[W]ww") %>]]

```dataview
TABLE
    meditated AS "Meditated",
    exercised AS "Exercised",
    read_book AS "Read Book"
FROM "2 Journal/Daily"
WHERE file.day.year = number(substring(string(this.file.name), 0, 4))
AND file.day.weekyear = number(substring(string(this.file.name), 6, 8))
SORT file.day
```


## Notes Created This Week

```dataview
TABLE highlights
FROM "2 Journal/Daily"
WHERE highlights != null
AND file.day.year = number(substring(string(this.file.name), 0, 4))
AND file.day.weekyear = number(substring(string(this.file.name), 6, 8))
SORT file.day
```



---



```dataview
TABLE meditations
FROM "2 Journal/Daily"
WHERE meditations != null
AND file.day.year = number(substring(string(this.file.name), 0, 4))
AND file.day.weekyear = number(substring(string(this.file.name), 6, 8))
SORT file.day
```



---



```dataview
TABLE foods
FROM "2 Journal/Daily"
WHERE foods != null
AND file.day.year = number(substring(string(this.file.name), 0, 4))
AND file.day.weekyear = number(substring(string(this.file.name), 6, 8))
SORT file.day
```

