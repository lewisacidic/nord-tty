# nord-tty
A theme for the Linux vconsole.  Because why not?


## Usage

When in a boring, normal Linux vconsole (e.g. by pressing `Ctrl`+`Alt`+`2`), source the file:

```sh
source nord-tty
```

Cool hint: you can put this in your `.{bash,zsh}rc`


## How does it work?

It uses the ANSI escape sequence to set the 16 console colors to those employed by nord.
Specifically, these are `\e]PXRRGGBB` where X is the color index, and RRGGBB is a color expressed in hexadecimal format.
These can be printed using `echo` with the `-en` flags.

