# Your `.gitignore` only needs _local

Add *_local* to the top gitignore file.

Keep development artifacts near where your code is.

No more tinkering with `.gitignore` files.

## Setup

```
$ cat <<EOF >> .gitignore
_local/
_local_*
EOF
```

Or, set up as a global `.gitignore` file:

```
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
