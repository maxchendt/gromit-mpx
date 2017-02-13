I modify a bit to fit Thinkpad that do not have an individual Pause Key (for example, Yoga 12, X230, X1 Yoga etc.)

1. swap shortcut key for "clear screen" and "toggle visibility".

2. for "redo last undone stroke", change the modify key from Shft to Ctrl

On Ubuntu, to build deb package

    sudo apt-get install --no-install-recommends git build-essential dh-autoreconf  debhelper cmake libgtk-3-dev libappindicator3-dev
    git clone -b Yoga12 https://github.com/maxchendt/gromit-mpx.git
    cd gromit-mpx
    dpkg-buildpackage -b -us -uc -i
    cd ..
    sudo dpkg -i gromit-mpx*.deb
Then, the hotkey is `F10`, and undokey is `Pause`. In my Yoga 12 (In Yoga 12, `Fn+P==Pause`, `Fn+B==Ctrl+Pause==Break`)

- F10:   toggle painting
- Ctrl+F10:   clear screen
- SHFT+F10:   toggle visibility
- Fn+P:   undo last stroke
- Fn+B:   redo last undone stroke




## Gromit-MPX

Gromit-MPX is a multi-pointer port of the original [Gromit annotation
tool](http://www.home.unix-ag.org/simon/gromit) by [Simon
Budig](mailto:simon@budig.de).

It enables graphical annotations with several pointers at once and is
A **lot** faster since it uses the XCOMPOSITE extension where
available.  Also, it does not inhibit Drag-and-Drop like the original
Gromit tool.



### What is it?

Gromit-MPX (GRaphics Over MIscellaneous Things) is a small tool to
make annotations on the screen.

Its main use is for making presentations of some application.
Normally, you would have to move the mouse pointer around the point of
interest until hopefully everybody noticed it.  With Gromit-MPX, you
can draw everywhere onto the screen, highlighting some button or area.


Similar tools for MS-Windows include *DemoHelper* (GPLv2 also), or
proprietary tools like *ZoomIt* and *ScreenMarker*.  For Compiz, there
is also the *Annotate* plugin, and the much-flashier *Firepaint (paint
fire on screen)* plugin.

see [Gromit-MPX](https://github.com/bk138/gromit-mpx) for more.

