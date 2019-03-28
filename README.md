# nord-tty
A theme for the Linux vconsole.  Because why not?


## Usage

When in a boring, normal Linux vconsole (e.g. by pressing `Ctrl`+`Alt`+`2`), source the file:

```sh
source nord-tty
```

Cool hint: you can put this in your `.{bash,zsh}rc`


## How does it work?

It sets the 16 console colors to those employed by nord with the appropriate ANSI escape sequences.
Specifically, these are `\e]PXRRGGBB` where X is the color index, and RRGGBB is a color expressed in hexadecimal format.
These can be printed using `echo` with the `-en` flags.


## Add to login screen

If you just can't wait until you log in for the nord-ttyness, you can add the commands to the start of `/etc/issue` to run before the login prompt:

```sh
cat nord-tty.issue /etc/issue > /tmp/issue && sudo mv /tmp/issue /etc/issue
```

