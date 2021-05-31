# Pomodoro Widget

## Usage

    cd ~/.config/awesome
    git clone git://github.com/zbioe/pomodoro-awesome.git pomodoro

In you rc.lua:

```lua
-- insert after beautiful.init("...")
pomodoro = require("pomodoro")

-- widget is now available in pomodoro:
```

Add it to your wibox:

```lua
mywibox[s].widgets = {
    pomodoro,
    mytextclock,
}
```

Add toggle pomodoro to keybinding

```lua
awful.key({modkey, "Shift"}, "p",
    function()
        pomodoro:toggle()
    end, {description = "Toggle Pomodoro", group = "Applications"}),
```

Add status pomodoro to keybinding

```lua
awful.key({modkey, "Shift"}, "p",
    function()
        pomodoro:status()
    end, {description = "Status Pomodoro", group = "Applications"}),
```

## Customization

If you want change the default icon, you can use beautiful:

    beautiful.pomodoro_icon_none = '/your/path/to/pomodoro/icon'
    beautiful.pomodoro_icon_start = '/your/path/to/pomodoro/icon'
    beautiful.pomodoro_icon_end = '/your/path/to/pomodoro/icon'

## License

Copyright 2010-2012 François de Metz

            DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
                    Version 2, December 2004

    Copyright (C) 2012 François de Metz

    Everyone is permitted to copy and distribute verbatim or modified
    copies of this license document, and changing it is allowed as long
    as the name is changed.

            DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
    TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION

    0. You just DO WHAT THE FUCK YOU WANT TO.
