# What
habeam allows you to interface with with Home Assistant REST API via
get or post requests.

# Why
habeam gives me the ability to toggle entities from a script. This means
I can assign hotkeys to trigger this script and so toggling lights is
just a click away when sat at my desk.

On MacOS I use Keyboard Maestro to create these macros and assign them
to function keys F13, F14, F15 on the Tweaker Macro Pad.

# How
The script uses argparse to take a set of flags and passes that data to
a get or post request.

# Help
```
usage: habeam [-h] -u URL -t TOKEN [-m {g,p}] -e ENTITY [-c {on,off,toggle}]

Home Assistant API Controller

optional arguments:
  -h, --help            show this help message and exit

Connection:
  -u URL, --url URL     Home Assistant Server URL
  -t TOKEN, --token TOKEN
                        Home Assistant Long Lived Token
  -m {g,p}, --method {g,p}
                        Specify The Method i.e GET / POST. Default Post

Entity:
  -e ENTITY, --entity ENTITY
                        Home Assistant Entity ID
  -c {on,off,toggle}, --control {on,off,toggle}
                        Control Action. Default Toggle

Any Questions feel free to reach out via support@ahmza.com
```

# Notes
- [Tweaker Macro Pad](https://blog.ahmza.com/posts/tweaker-macro-pad)
