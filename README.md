# Magnet2Torrent

A command line tool that converts magnet links into .torrent files.

## Requirements
This fork has only been tested with:
* python3 3.11.8
* python3-libtorrent (libtorrent-rasterbar version 2.0.10)

### Install libtorrent-python on Mac

    brew install libtorrent-rasterbar --with-python

### Install python-libtorrent on Ubuntu
    sudo apt-get install python-libtorrent -y

## Usage

    usage: Magnet2Torrent.py [-h] -m MAGNET [-o OUTPUT] [--rewrite-file]
                             [--no-rewrite-file] [--skip-file] [--open-file]

A command line tool that converts magnet links into .torrent files

Optional arguments:

    -h, --help            Show this help message and exit.
    -m MAGNET, --magnet MAGNET
                            The magnet url.
    -o OUTPUT, --output OUTPUT
                            The output torrent file name.
    --rewrite-file        Rewrite torrent file if it already exists (default).
	--no-rewrite-file     Create a new filename if torrent exists.
	--skip-file           Skip file if it already exists.
    --open-file           Open file after converting.

## Example usage

    python MagnetToTorrent.py -m <magnet link> [torrent file]

    python Magnet2Torrent.py -m "magnet:?xt=urn:btih:49fbd26322960d982da855c54e36df19ad3113b8&dn=ubuntu-12.04-desktop-i386.iso&tr=udp%3A%2F%2Ftracker.openbittorrent.com" -o ubunut12-04.iso

## Licenses
All code is licensed under the [GPL version 3](http://www.gnu.org/licenses/gpl.html)
