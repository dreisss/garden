---
created_at: 2024-08-23
tags:
  - literature/book-collection
  - subject/mathematics
title: Fundamentos de Matemática Elementar
authors:
  - "[[Gelson Iezzi]]"
  - "[[Carlos Murakami]]"
publisher: "[[Editora Saraiva]]"
isbn:
  - OCLC:817775025
cover: https://scontent.fstm2-1.fna.fbcdn.net/v/t1.6435-9/105546262_713850585846519_1432733713419895387_n.jpg?_nc_cat=108&ccb=1-7&_nc_sid=06a7ca&_nc_ohc=tj2kbfhq8z4Q7kNvgERzOzf&_nc_ht=scontent.fstm2-1.fna&oh=00_AYAYLVdfIvC-XzPP8RFfdIrM4D5QzKKQ611bE5hAT5tOig&oe=66F01C13
source: 
physical: true
read_start: 
read_finish: 
status: read
rating: favorite
aliases:
  - FME - v. 01
cssclasses:
  - cover-align-center
---

![cover|200](https://scontent.fstm2-1.fna.fbcdn.net/v/t1.6435-9/105546262_713850585846519_1432733713419895387_n.jpg?_nc_cat=108&ccb=1-7&_nc_sid=06a7ca&_nc_ohc=tj2kbfhq8z4Q7kNvgERzOzf&_nc_ht=scontent.fstm2-1.fna&oh=00_AYAYLVdfIvC-XzPP8RFfdIrM4D5QzKKQ611bE5hAT5tOig&oe=66F01C13)

#### `= this.title`

> [!example] subjects
> ```dataviewjs
> dv.list(dv.current().file.tags.filter(tag => tag.startsWith("#subject") && tag != "#subject").sort())
> ```

 É uma coleção de livros de física divididos em onze volumes:

```dataviewjs
dv.list([1].map(n => {
	const name = `Fundamentos de Matemática Elementar - Vol. 0${n}`
	
	const title = dv.pages('').where(p => p.file.name == name).file.frontmatter.title[0]
	
	return `[[${name}|${title}]]`
}))
```

