---
created_at: 2024-08-22
tags:
  - literature/book-colection
  - subject/physics
title: The Feynman Lectures on Physics
authors:
  - "[[Richard P. Feynman]]"
  - "[[Robert B. Leighton]]"
  - "[[Matthew Sands]]"
publisher: "[[bookman]]"
isbn: 
cover: https://pictures.abebooks.com/inventory/md/md30941665532.jpg
source: 
physical: true
read_start: 
read_finish: 
status: reference reading
rating: favorite
aliases:
  - Feynman Lectures - v. 01
cssclasses:
  - cover-align-center
---

![cover|200](https://pictures.abebooks.com/inventory/md/md30941665532.jpg)

#### `= this.title`

> [!example] subjects
> ```dataviewjs
> dv.list(dv.current().file.tags.filter(tag => tag.startsWith("#subject") && tag != "#subject").sort())
> ```
 
 É uma coleção de livros de física divididos em três volumes:

```dataviewjs
dv.list([1, 2, 3].map(n => {
	const name = `${dv.current().file.name} - Vol. 0${n}`
	const title = dv.pages('').where(p => p.file.name == name).file.frontmatter.title[0]
console.log(name)
	
	return `[[${name}|${title}]]`
}))
```
