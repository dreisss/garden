<%"---"%>
created_at: {{date}}
tags: <%=`\n  - literature/book${book.categories == undefined ? "" : book.categories.map(category=>`\n  - subject/${category}`).join('')}`%>
title: <%=`"${book.title}${book.subtitle == undefined ? "" : `: ${book.subtitle}`}"`%>
authors: <%=book.authors.map(author=>`\n  - "[[${author}]]"`).join('')%>
publisher: <%=book.publisher == undefined ? "" : book.publisher%>
isbn:<%=`\n  - "${book.isbn10}"\n  - "${book.isbn13}"`%>
cover: {{coverUrl}}
source:
physical: false
read_start:
read_finish:
status: unread
rating: ok
aliases:
cssclasses: cover-align-center
<%"---"%>
![cover|200](<%=book.coverUrl%>)

