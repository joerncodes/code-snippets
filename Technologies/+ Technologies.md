```dataviewjs
const pages = dv.pages('"Technologies" AND !"Technologies/+ Technologies"');

dv.table(["Technology", "Snippet Count", "Random Snippet"], pages.map((page) => {
 	return[
		dv.fileLink(page.file.name),
		page.file.inlinks.length,
		page.file.inlinks[page.file.inlinks.length * Math.random() | 0]
	];
}));
```
