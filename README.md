# hit

Highlight keywords, that's all.


## How to use

Highlight keywords in terminal, from a single file

```bash
> hit Highlight ./README.md
```

Read from stdin

```bash
> curl -s https://sh.rustup.rs | hit RUSTUP
```

`hit` can use regular expressions for highlighting keywords

```bash
> curl -s https://sh.rustup.rs | hit "[Rr]ust"
```

`hit` can be combined with `tail -f` to continously monitor a given file for highlight keywords

```bash
> tail -f /var/log/nginx.log | hit 401
```


## Installation

### From source

```
$ cargo install hit
```
