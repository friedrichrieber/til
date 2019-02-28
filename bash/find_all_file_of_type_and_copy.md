# Find all Files of one File Type and Copy to a Directory

This Bash command shoudl find all files of one kind and copy them to another directory.

This example finds all ``` .vhd ``` files and copys them to the directory ``` friedrich_tools ```.

```bash
find -iname '*.vhd' -exec cp {} ./friedrich_tools/ \;
```
