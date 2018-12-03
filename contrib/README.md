
Debian
====================
This directory contains files used to package pinecoind/pinecoin-qt
for Debian-based Linux systems. If you compile pinecoind/pinecoin-qt yourself, there are some useful files here.

## pinecoin: URI support ##


pinecoin-qt.desktop  (Gnome / Open Desktop)
To install:

	sudo desktop-file-install pinecoin-qt.desktop
	sudo update-desktop-database

If you build yourself, you will either need to modify the paths in
the .desktop file or copy or symlink your pinecoinqt binary to `/usr/bin`
and the `../../share/pixmaps/pinecoin128.png` to `/usr/share/pixmaps`

pinecoin-qt.protocol (KDE)

