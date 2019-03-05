# Find all Files of one File Type and Copy to a Directory

This Bash command shoudl find all files of one kind and copy them to another directory.

This example finds all ``` .pdf ``` files and copys them to the directory ``` directory ```.

```bash
find -iname '*.pdf' -exec cp {} ./directory/ \;
```
