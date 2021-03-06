# ncgopher

`ncgopher` is a gopher and gemini client for the modern internet. It uses
ncurses and is written in Rust.


## gopher

Gopher was developed in 1991 at the University of Minnesota, and named
after the school's mascot. Gopher is a menu-driven interface that
allows a user to browse for text information served off of various
gopher servers.


## gemini

Gemini is a new application-level internet protocol for the distribution
of arbitrary files, with some special consideration for serving a
lightweight hypertext format which facilitates linking between files.


## Screenshot

Obligatory screenshot:

![img](./screenshots/ncgopher.png "Screenshot of NcGopher")

![img](./screenshots/ncgopher-darkmode.png "Screenshot of NcGopher")


## Features

-   Gopher and gemini support
-   Ncurses interface
-   Keyboard commands for navigation
-   Bookmarks support including custom title
-   History of visited gopher holes
-   Download of text files and gophermaps (Save as&#x2026;)
-   Download of binary files
-   Menu for easy configuration
-   Mouse support in some terminals
-   TLS support
-   Darkmode!
-   Common search providers in search menu for quick access
-   External commands for HTML, images and Telnet


## Installation

`ncgopher` has no fancy installation process right now. Make sure to install
rust on your system, but the latest release can be installed through cargo:

    cargo install ncgopher

To install the latest development version:

    git clone https://github.com/jansc/ncgopher.git
    cd ncgopher
    cargo build
    cargo run


## Key bindings

During alpha, the keybindings are not configurable and many operations
are still not implemented.

    |------------+--------------------------------|
    | Key        | Command                        |
    |------------+--------------------------------|
    | Arrow keys | Move around in text            |
    | Enter      | Open the link under the cursor |
    | Esc        | Go to menubar                  |
    | Space      | Scroll down one page           |
    | g          | Open new URL                   |
    | b          | Navigate back                  |
    | q          | Close application              |
    | s          | Save current page              |
    | r          | Reload current page            |
    | i          | Show link under cursor         |
    | a          | Add bookmark for current page  |
    | n          | Go to next link                |
    | p          | Go to previous link            |
    | j          | Move one line down             |
    | k          | Move one line up               |
    |------------+--------------------------------|

## Mouse support

`ncgopher` supports mouse interaction for menus and buttons in dialogs.
If you want to select text, most terminal support selection while 
pressing `SHIFT`.


## Debugging

The software is still in beta, and it is also my first application
written in Rust. Expect lots of bugs and badly written Rust code.

If the application crashes, I'd be interested in a backtrace. Start
the application with `RUST_BACKTRACE=1 cargo run`.  There is also a
debug view that can be activated with the `~`-key.


## License

`ncgopher` is licensed under the BSD 2-clause license.

Copyright (c) 2020, Jan Schreiber. Parts of the status bar
implementation are Copyright (c) 2019, Henrik Friedrichsen

