# Counting files in directory


To count specific files in the directory you can use the following command 

```sh

ls *.<file_extension> | wc -l

```
lets say if you want to see how many css files you have in a directory you might use this command as 

```sh

ls *.css | wc -l

```