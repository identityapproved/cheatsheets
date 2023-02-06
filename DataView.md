___
draft: true
___

```dataview
table file.ctime.day as Day, file.ctime.month as Month, file.ctime.year as Year 
FROM ""
where file.ctime > (date(now) - dur(8 days))
SORT file.ctime desc
```
