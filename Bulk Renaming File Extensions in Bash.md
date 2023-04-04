Technology::[[Bash]]
    
```bash
for f in \*.txt; do 
	mv -- "$f" "${f%.txt}.md"
done
```


