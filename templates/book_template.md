<%"---"%>
created_at: {{date}}
tags: book
title: "{{title}}"
subtitle: "{{subtitle}}"
authors: <%=book.authors.map(author=>`\n  - "[[${author}]]"`).join('')%>
subjects: <%=book.categories.map(category=>`\n  - ${category}`).join('')%>
publisher: {{publisher}}
published_at: {{publishDate}}
pages: {{totalPage}}
isbn:<%=`\n  - "${book.isbn10}"\n  - "${book.isbn13}"`%>
cover: {{coverUrl}}
source:
aliases:
status: unread
<%"---"%>
![cover|200](<%=book.coverUrl%>)

## Outline
