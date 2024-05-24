# Your `.gitignore` only needs _local

Add *_local* to the global gitignore file.

Keep development artifacts near where your code is.

Never touch `.gitignore` files again.

## Setup


```sh
$ cat <<EOF >> ~/.gitignore
_local/
_local_*
EOF

$ git config --global core.excludesfile ~/.gitignore
```
  
## Usage

```
$ mkdir _local
$ cc main.c -o _local/main
```
