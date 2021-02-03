# TIL (Things I discover Linux/Programming/Automation)


xargs -n 1 curl -sL < 2018.txt | grep -Eo "<title>.*</title>" The command to extract links using curl

curl -sL https://news.ycombinator.com/item\?id\=18740939 | grep -Eo 'href="(https|http):[^\"]+"' Command to extract the links from hackernews

grep -aEo "<title>.*</title>" -a option process binary file https://unix.stackexchange.com/questions/335716/grep-returns-binary-file-standard-input-matches-when-trying-to-find-a-string

use ``` backticks to run a command in bash


## 2021-01-29
- you can use `?*` to match the rest of the characters when moving the files 
In order to delete a branch on git locally you can use `git branch --delete <branchname>` and if you want to do it remotely you can do `git push --delete <branchname>`

## 2021-02-21
- To count specific files in the directory you can use the following command `ls *.<file_extension> | wc -l`. lets say if you want to see how many css files you have in a directory you might use this command as `ls *.css | wc -l`

