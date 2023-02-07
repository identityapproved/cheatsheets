---
draft: true
---

```dataview
list from #terminal 
```
```dataview
task from "Kanbans"
```

```dataview
TABLE
	tag as "Shortcuts"
FROM "Shortcuts"
```

```dataview
TABLE 
	file.ctime.day as Day, 
	file.ctime.month as Month, 
	file.ctime.year as Year 
FROM ""
WHERE file.ctime > (date(now) - dur(8 days))
SORT file.ctime desc
```
