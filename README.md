# TIL (Things I discover Linux/Programming/Automation)


xargs -n 1 curl -sL < 2018.txt | grep -Eo "<title>.*</title>" The command to extract links using curl

curl -sL https://news.ycombinator.com/item\?id\=18740939 | grep -Eo 'href="(https|http):[^\"]+"' Command to extract the links from hackernews

grep -aEo "<title>.*</title>" -a option process binary file https://unix.stackexchange.com/questions/335716/grep-returns-binary-file-standard-input-matches-when-trying-to-find-a-string

use ``` backticks to run a command in bash


## 2021-01-29
- you can use `?*` to match the rest of the characters when moving the files 
In order to delete a branch on git locally you can use `git branch --delete <branchname>` and if you want to do it remotely you can do `git push --delete <branchname>`

## 2021-02-2
- To count specific files in the directory you can use the following command `ls *.<file_extension> | wc -l`. lets say if you want to see how many css files you have in a directory you might use this command as `ls *.css | wc -l`

## 2021-02-04
- We can use this command to generate a `grub` configuration file, `sudo grub-mkconfig -o /boot/grub/grub.cfg`,As, `grub-mkconfig` scans hardrives for bootable operating systems such as windows,mac or linux distros

## 2021-02-11

To open workspaces on specific windows when using `i3` window mananger use the following `assign [class="<use your program name here e.g. - Firefox>"] $workspace<eg. 5>` and refresh `i3-msg reload`

## 2021-02-12

In order to resize images using command you can use the `convert` command. `convert img.jpg -resize 200x200 img-1.jpg` and you can also convert to different extenstions using `convert` command. `convert img.png img.jpg`


## 2021-02-27
- To add a printer on linux use `CUPS` web admin `http://localhost:631/`
## 2021-02-19

`fuser -k <port_name>/tcp` use `fuser` to kill specific ports on linux

jinja line break `{% autoescape false %} {{ org.backgroundInfo | replace(‘\n’, ‘<br>’) }} {% endautoescape %}`

In order to save a file with root permission using vim you can do `:w !sudo tee %`  
