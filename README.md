fujinet-tnfs-fuse
=================

An attempt to move TNFS FUSE driver into Python3 realm and currently supported FUSE bindings for Python.

This is all thanks to the renewed TNFS interest from https://fujinet.online Atari 8-bit community.

- [x] Client is running with Python3 now.
- [ ] FUSE driver not working yet

tnfs_client.py usage
--------------------
`python3 tnfs_client.py [<tnfs-server>] [<tnfs-port>]`

Default `<tnfs-server>` is `vexed4.alioth.net`
Default `<tnfs-port>` is `16384`

Available commands:

`ls [<path>]` - list directory contents

`ls -l [<path>]` - detailed list

`cd <path>` - change directory

`pwd` - show current directory

`mkdir <path>` - create directory

`rmdir <path>` - delete directory

`get <remote filename>[,<local filename>]` - download from tnfs server

`put <local filename>[,<remote filename>]` - upload to tnfs server

`quit` - exit to DOS


The original message from Author below:

spectranet-tnfs-fuse
====================

Linux FUSE filesystem driver for use with the TNFS filesystem that the ZX Spectranet uses.
I made this only because I wanted easy access to vexed4.alioth.net from my computer, and
the corresponding directories in SVN were empty.

Quality is to be considered Alpha. If it eats your data, I take no responsibility.

I'm creating this repository here because I can't for the life of me figure out how to contact
Winston, the creator of the Spectranet Ethernet interface for the ZX Spectrum, to include this
into his repository.

For more information about the Spectranet interface go here: http://spectrum.alioth.net/doc/index.php/Main_Page
