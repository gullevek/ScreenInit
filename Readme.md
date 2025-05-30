# Sceen init scripts

Init screens from config files

`screen_init.sh <config>`

## Config file layout

```txt
<screen session name>
<window name>#<command>;<command>;
#
;<ignored line>
```

- `screen session name` is the name you use for gstting the screen session name, see `screen -ls`. Must be Alphanumeric without spaces and cannot be empty
- `window name` is the name for this window
- `command` can be any comamnd sequence separated by `;`. If nothing given default `^C` shell is used
- If there is only a `#` an empty unnamed window is opened
- if a line starts with `;` it is skipped
- empty lines are ignored
