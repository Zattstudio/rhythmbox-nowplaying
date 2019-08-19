# Now Playing - Rhythmbox plugin - 0.2

Rhythmbox plugin that prints artist, song, and rating to a text file.
Updated version of sagotsky/rhythmbox-nowplaying-text.
In addition, a format file was added for custom formatting of the output file.


## Installation

First, open the terminal and issue the following commands:

    mkdir -p ~/.local/share/rhythmbox/plugins
    cd ~/.local/share/rhythmbox/plugins
    git clone https://github.com/Zattstudio/rhythmbox-nowplaying.git

Then enable the plugin within Rhythmbox by going to "Edit", selecting "Plugins"
and then checking the "Now Playing Text" plugin.

## Usage

The plugin will output a file in the home folder with the name **.rhythmbox-current.out**
If you do not see this file you might have to enable 'show hidden files' in your file manager.

The format template is located at ~/.local/share/rhythmbox/plugins
/rhythmbox-nowplaying/FORMAT.
DO NOT change the name of this file or delete it.

You can use **[Artist]**, **[Album]**, **[Genre]** and **[Title]** (with the square brackets)
for formatting. These tags will just be replaced with actual data. You can add
any kind of characters around them. 
