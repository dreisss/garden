---
created_at: 2024.08.22 (Thu)
tags:
  - page
aliases: 
cssclasses:
  - banner
  - banner-fade
  - cards
  - cards-cover
  - cards-2-3
  - checkbox-adjusts
  - library-adjusts
---

My personal library with books, articles, blog posts, etc.

```dataviewjs
const literature = dv.pages('#literature').where(() => true)

dv.table([
	"cover", "title", "physically", "status", "rating", "tags"
	], literature.map(l => {
	let status

	if (l.status == "unread") (status = "!")
	if (l.status == "read") (status = "x")
	if (l.status == "reading") (status = "/")
	if (l.status == "reference reading") (status = "n")
	if (l.status == "not finished") (status = "!")

	let rating

	if (l.rating == "very bad") (rating = "c")
	if (l.rating == "bad") (rating = "d")
	if (l.rating == "ok") (rating = "p")
	if (l.rating == "good") (rating = "u")
	if (l.rating == "favorite") (rating = "*")

	const tags = l
		.tags.filter(t => t.startsWith("subject"))
		.map(tag => `- #${tag}`)

	return [
		`![](${l.cover})`,
		`###### ${l.file.link}`,
		`- [${l.physical ? "p" : "c"}] physically`,
		`- [${status}] ${l.status}`,
		`- [${rating}] ${l.rating}`,
		tags
	]
}).sort(l => l[1]))
```

![[library.avif|banner]]
