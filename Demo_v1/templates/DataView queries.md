

https://blacksmithgu.github.io/obsidian-dataview/queries/query-types/


## Заметки за сегодня

````markdown
```dataview
LIST
FROM !"templates"
WHERE date(today) = file.mday
SORT file.mtime DESC
```
````


## Поиск по тегам
````markdown
```dataview
TABLE file.mday as "modification date"
FROM #TBD
sort file.mday DESC
```
````

## Поиск по таскам

````markdown
```dataview
TASK
```
````

````markdown
```dataview
TASK
WHERE !completed
GROUP BY file.link
```
````