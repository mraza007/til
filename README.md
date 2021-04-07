# TIL (Things I discover Linux/Programming/Automation)


# Linux

xargs -n 1 curl -sL < 2018.txt | grep -Eo "<title>.*</title>" The command to extract links using curl

curl -sL https://news.ycombinator.com/item\?id\=18740939 | grep -Eo 'href="(https|http):[^\"]+"' Command to extract the links from hackernews

grep -aEo "<title>.*</title>" -a option process binary file [link to sol](https://unix.stackexchange.com/questions/335716/grep-returns-binary-file-standard-input-matches-when-trying-to-find-a-string)
use ``` backticks to run a command in bash

-

- We can use this command to generate a `grub` configuration file, `sudo grub-mkconfig -o /boot/grub/grub.cfg`,As, `grub-mkconfig` scans hardrives for bootable operating systems such as windows,mac or linux distros

- To open workspaces on specific windows when using `i3` window mananger use the following `assign [class="<use your program name here e.g. - Firefox>"] $workspace<eg. 5>` and refresh `i3-msg reload`

- In order to resize images using command you can use the `convert` command. 
`convert img.jpg -resize 200x200 img-1.jpg` and you can also convert to different extenstions using `convert` command. `convert img.png img.jpg`

- To add a printer on linux use `CUPS` web admin `http://localhost:631/`

- `fuser -k <port_name>/tcp` use `fuser` to kill specific ports on linux

- In order to save a file with root permission using vim you can do 
`:w !sudo tee %`

- This commands `sudo netstat -plunt |grep post` outputs the port on which postgres db is running on

- `chmod -x` allows you to revert the executable created by `chmod +x`

- you can use `?*` to match the rest of the characters when moving the files 



## Git

In order to delete a branch on git locally you can use 
`git branch --delete <branchname>` and if you want to do it remotely you can do `git push --delete <branchname>`

To delete git commit history do the following
- `git checkout --orphan <branch_name>`
- `git add -A`
- `git commit --all -m "a message"`
- `git branch -D <delete the main branch>`
- `git branch -m <rename the new branch to main branch>`
- `git push -f origin <new branch>`


## Python

jinja line break 
`{% autoescape false %} {{ org.backgroundInfo | replace(‘\n’, ‘<br>’) }} {% endautoescape %}`

