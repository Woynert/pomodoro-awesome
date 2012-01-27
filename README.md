# Pomodoro Widget

### Now with sounds!

Forked off francois2metz: still 99% his original code.

Sounds downloaded from: http://www.grsites.com, and claim to be:

  The background textures, fonts and sound effects found on this site
  were not created by GRSites, but were obtained from various sources
  on the internet that described these graphics as freeware. They are
  free to use for personal and commercial use.



## Usage

Requires mpg321 to play the sounds.

    sudo apt-get install mpg321

Then

    cd ~/.config/awesome
    git clone git://github.com/danverbraganza/pomodoro-awesome.git pomodoro

In you rc.lua:


    // insert after beautiful.init("...")
    require("pomodoro")

    -- widget is now available via:
    pomodoro()

Add it to your wibox:

    mywibox[s].widgets = {
        pomodoro(),
        mytextclock,
    }

## Customization

If you want change the default icon, you can use beautiful:

    beautiful.pomodoro_icon = '/your/path/to/pomodoro/icon'

## License

Copyright 2010-2011 François de Metz

            DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
                    Version 2, December 2004

    Copyright (C) 2004 Sam Hocevar <sam@hocevar.net>

    Everyone is permitted to copy and distribute verbatim or modified
    copies of this license document, and changing it is allowed as long
    as the name is changed.

            DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
    TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION

    0. You just DO WHAT THE FUCK YOU WANT TO.
