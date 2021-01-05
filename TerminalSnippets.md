# Terminal Snippets

## Show timestamp with ping
You can get a unix timestamp with `ping -D`. To get a nice timestamp, use:

```
ping localhost | while read pong; do echo "$(date): $pong"; done
```

## Copy current path into clipboard
Note: Only using `pwd` adds a newline character at the end. 
`printf` in combinatio with string formatting provides a safe way to get the output of `pwd`

```
printf '%s' $(pwd) | pbcopy
```

Source: https://stackoverflow.com/a/3483565
