<h1 align="center">NOTFLIX</h1>
<p align="center">f@#k netflix use notflix a tool which search magnet links and stream it with webtorrent</p>

##
<p align="center">
<img src="./preview.gif" alt="Video Preview" width="500px">
</p>

> Watch my video on this - [bugswriter's notflix](https://youtu.be/RFJCL9C46Mc)

### How does this work?

This is a shell script. It scrapes 1337x and gets the magnet link.
After this it uses [webtorrent](https://webtorrent.io/) to stream the video from the magnet link.
For scraping, the script uses simple gnu utils like sed, awk, paste, cut.

## Requirements
* [cygwin](https://cygwin.com/install.html) - Install cygwin then install required pkgs by selecting them in initial setup.
```
binutils fzf git
```

* [vlc](https://www.videolan.org/vlc/download-windows.html) - Install vlc media player.

## Using install script

* [Install](https://github.com/mmtrt/notflix-nyaa-termux/raw/win/install) - Install script which automates all below instructions.
```
curl -sL "https://github.com/mmtrt/notflix-nyaa-termux/raw/win/install" > install && chmod +x install && ./install
```
## Using manual method

* [nodejs](https://nodejs.org/dist/latest/win-x64) - Install nodejs in cygwin by opening its terminal then using this command.
```
curl -sL "https://nodejs.org/dist/latest/win-x64/node.exe" > /bin/node.exe && chmod +x /bin/node.exe
```
* [npm-cli](https://github.com/npm/cli) - Install npm-cli

```
git clone --depth 1 https://github.com/npm/cli.git
```

```
(cd cli/node_modules ; rm -rf libnpmfund ; cp -r ../workspaces/libnpmfund/ .)
```

```
(cd cli/node_modules/@npmcli ; rm -rf arborist ; cp -r ../../workspaces/arborist/ .)
```

```
(cd cli ; node bin/npm-cli.js install -g npm ; cd .. ; rm -rf ./cli)
```

* [webtorrent-cli](https://github.com/webtorrent/webtorrent-cli) - A tool to stream torrent.
```
npm install webtorrent-cli -g
```

## Installation

### notflix
cURL **notflix** to your **$PATH** and give execute permissions.

```
curl -sL "https://github.com/mmtrt/notflix-nyaa-termux/raw/win/notflix" > /bin/notflix && chmod +x /bin/notflix
```
- To update, just do `curl` again, no need to `chmod` anymore.
- To uninstall, simply remove `notflix` from your **$PATH**, for example `rm -f /bin/notflix.

### nyaa
cURL **nyaa** to your **$PATH** and give execute permissions.

```
curl -sL "https://github.com/mmtrt/notflix-nyaa-termux/raw/win/nyaa" > /bin/nyaa && chmod +x /bin/nyaa
```
- To update, just do `curl` again, no need to `chmod` anymore.
- To uninstall, simply remove `nyaa` from your **$PATH**, for example `rm -f /bin/nyaa.

## License
This project is licensed under [GPL-3.0](https://raw.githubusercontent.com/Illumina/licenses/master/gpl-3.0.txt).

