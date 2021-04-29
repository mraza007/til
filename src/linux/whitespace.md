# A simple command to turn whitespaces into `_`

```bash

for f in *; do mv "$f" `echo $f | tr ' ' '_'`; done

```
