# Sceen init scripts

Init screens from config files

`screen_init.sh <config>`

## Config file layout

```
<screen title>
<window name>#<command>
```

`screen title` is the name you use for getting the screen, see `screen -ls`. Must be Alphanumeric without spaces.
`window name` is the name for this window
`command` can be any comamnd sequence separated by `;`. If nothing given default `^C` shell is used
