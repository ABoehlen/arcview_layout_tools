# arcview_layout_tools
Layout Tools is an Avenue extension used in ArcView GIS that provides many useful functions for working with layouts.

## Purpose
Layout Tools includes tools for convenient editing layouts. There are some general tools and a command line which has to be used for all the other tools: Type `help` to open a list of all available commands and their functions:

* `cp`: Copies a layout
* `delhd`: Deletes header and footer for the chosen layouts
* `dels`: Deletes selected features
* `def`: Shows dialog to select the default value table
* `fi`: Imports textfiles
* `fis`: Imports textfiles preformatted
* `go`: Switches guides on (for the active layout)
* `gom`: Switches guides on (for many layouts)
* `gf`: Switches guides off (for the active layout)
* `gfm`: Switches guides off (for many layouts)
* `hd`: Creates header and footer for the active layout
* `hdm`: Creates header and footer for many layouts
* `help`: Shows this help page
* `help <cmd>`: Shows the help for the chosen command
* `lytimp`: Imports a layout from an ODB file 
* `lytexp`: Exports one or more layouts into an ODB file
* `mrg`: Shows recommended margins
* `mx<value>`: Moves the selected elements on the x axis
* `my<value>`: Moves the selected elements on the y axis
* `new`: Creates a new layout document
* `ol`: Imports text for ordered list
* `ols`: Imports text preformatted for ordered list
* `regm`: Creates registration marks
* `selall`: Selects all elements on the active layout
* `ti`: Imports text
* `tis`: Imports text preformatted
* `ul`: Imports text for unordered list
* `uls`: Imports text preformatted for unordered list
* `wd`: Shows dialog to select the working directory
* `unselall`: Unselect all selected elements
* `zoomex`: Zoom to exportview

## Background
ESRI's ArcView GIS is a rather old (1995 – 2002), but for many purposes still useful GIS application. Due to its age it's very fast on modern hardware and has full support for the still widely used vector data format _Shape_ (SHP).

Avenue is ArcView's built-in object oriented scripting language. "By using Avenue, you can customize the program and further extend its power", describes Amir H. Razavi the language's purpose in his 1999 book \[1\].

## System requirements
An ArcView GIS 3.x installation is required.

## Installation
Download the repository into your desired directory:

```
cd <directory>
git clone https://github.com/ABoehlen/arcview_layout_tools
```

* Copy LayoutTools.avx into the ext32 directory of your ArcView installation.
* Copy default_values.dbf into a directory of your choice if it doesn't exist already. The same file is used by https://github.com/ABoehlen/arcview_editor
* Open ArcView GIS with a new empty project or with an existing one.
* Choose File –> Extensions
* Turn on the Extension Editor and close the Extension dialog again.
* In the View documents open an existing view or create a new one.
* In the button list of the View document GUI click on the new button "Starts LayoutTools toolbar". The toolbar should open. As well opens the dialog where you have to select the default_values.dbf table file.

## License

This project is licensed under the MIT License - see the LICENSE file for details

***

## Literature
\[1\] Razavi, Amir H.: ArcView GIS Developer's Guide, 1999

