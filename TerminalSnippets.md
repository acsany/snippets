# Terminal Snippets

## Show timestamp with ping
You can get a unix timestamp with `ping -D`. To get a nice timestamp, use:

```
ping localhost | while read pong; do echo "$(date): $pong"; done
