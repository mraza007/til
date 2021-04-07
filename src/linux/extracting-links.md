# Extract Links using `CURL`

```sh
xargs -n 1 curl -sL < 2018.txt | grep -Eo "<title>.*</title>" The command to extract links using curl
```

```sh
curl -sL https://news.ycombinator.com/item\?id\=18740939 | grep -Eo 'href="(https|http):[^\"]+"' Command to extract the links from hackernews
```

```sh
grep -aEo "<title>.*</title>" 
```

`-a` option to process binary file [link to sol](https://unix.stackexchange.com/questions/335716/grep-returns-binary-file-standard-input-matches-when-trying-to-find-a-string)



use ``` backticks to run a command in bash
