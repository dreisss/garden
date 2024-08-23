---
created_at: 2024-08-23
tags:
  - literature/book-collection
  - subject/physics
title: Curso de Física Básica
authors:
  - "[[Herch Moysés Nussenzveig]]"
publisher: "[[Editora Blucher]]"
isbn: []
cover: https://zonadaeletrica.com.br/wp-content/uploads/2019/09/fisica-basica-vol-moyses-nussenzveig-4ed-213x300.jpg
source: 
physical: true
read_start: 
read_finish: 
status: unread
rating: favorite
aliases:
  - Fisica Básica
cssclasses:
  - cover-align-center
---

![cover|200](https://zonadaeletrica.com.br/wp-content/uploads/2019/09/fisica-basica-vol-moyses-nussenzveig-4ed-213x300.jpg)

#### `= this.title`

> [!example] subjects
> ```dataviewjs
> dv.list(dv.current().file.tags.filter(tag => tag.startsWith("#subject") && tag != "#subject").sort())
> ```

É uma coleção de livros de física divididos em quatro volumes:

```dataviewjs
dv.list([1, 2, 3, 4].map(n => {
	const name = `Curso de Física Básica - Vol. 0${n}`
	
	const title = dv.pages('').where(p => p.file.name == name).file.frontmatter.title[0]
	
	return `[[${name}|${title}]]`
}))
```





