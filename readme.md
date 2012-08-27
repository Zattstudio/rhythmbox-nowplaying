# Now Playing Text - Rhythmbox plugin - 0.2

Rhythmbox plugin that prints artist, song, and rating to a text file.  Forked from rhythmbox-nowplaying-xml
Tested with Rhythmbox Version 2.96

## Installation

First, open the terminal and issue the following commands:

    mkdir -p ~/.local/share/rhythmbox/plugins
    cd ~/.local/share/rhythmbox/plugins
    git clone git@github.com:rethab/rhythmbox-nowplaying-text.git

Then enable the plugin within Rhythmbox by going to "Edit", selecting "Plugins"
and then checking the "Now Playing Text" plugin.

## Xmobar

To use this with xmobar (which is what I forked the xml version for), create a fifo:

  mkfifo ~/.rhythmbox.out
Add a PipeReader to your .xmobarrc

  , Run PipeReader    "/home/sagotsky/.rhythmbox.out" "music"
And add %music% to your template
