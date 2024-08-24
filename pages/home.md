---

created_at: 2024.08.23 (Fri)
tags:
  - page
aliases:
  - homepage
kanban-plugin: board
cssclasses:
  - page-adjusts
  - cards
  - cards-cover
  - cards-cols-5
  - cards-2-3

---

## 

- [ ] ## Recent
	 
	```dataviewjs
	dv.list(
		dv.pages('').sort(p => p.mtime, "desc").limit(5).file.link
	).reverse
	```


## 

- [ ] ![[daily.gif|120]]
	`=link(dateformat(date(today), "yyyy.MM.dd (ccc)"))`


## 

- [ ] ## Reading
	```dataviewjs
	const literature = dv.pages('#literature').where(l => {
		return [
			"reading", "not finished"
		].includes(l.file.frontmatter.status)
	})
	
	dv.table(["cover"], literature.map(l => {
		return [
			`![](${l.cover})`,
			l.file.link
		]
	}).sort(l => l[1]))
	```




%% kanban:settings
```
{"kanban-plugin":"board","list-collapse":[false,false,false],"show-checkboxes":false,"full-list-lane-width":false,"show-set-view":false,"show-view-as-markdown":false,"show-archive-all":false,"show-add-list":false,"hide-card-count":true}
```
%%