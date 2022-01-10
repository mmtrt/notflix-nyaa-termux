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
* [Termux](https://f-droid.org/en/packages/com.termux) - Install terminal app from f-droid then install required pkgs in Termux.
```
pkg up -y && pkg in binutils git nodejs python -y
```

* [webtorrent](https://webtorrent.io/) - A tool to stream torrent.
```
npm install webtorrent-cli -g
```
* [mpv-android](https://play.google.com/store/apps/details?id=is.xyz.mpv) - Install player from playstore then add mpv script in termux.
```
curl -sL "https://github.com/mmtrt/notflix-termux/raw/termux/mpv" -o ../usr/bin/mpv && chmod +x ../usr/bin/mpv
```

## Optional

* [MX Player](https://play.google.com/store/apps/details?id=com.mxtech.videoplayer.ad) - Install player from playstore then add MXPlayer script in termux.
```
curl -sL "https://github.com/mmtrt/notflix-termux/raw/termux/mxplayer" -o ../usr/bin/mpv && chmod +x ../usr/bin/mpv
```
* [VLC](https://play.google.com/store/apps/details?id=org.videolan.vlc) - Install player from playstore then add VLC script in termux.
```
curl -sL "https://github.com/mmtrt/notflix-termux/raw/termux/vlc" -o ../usr/bin/mpv && chmod +x ../usr/bin/mpv
```
* [Mi Video](https://play.google.com/store/apps/details?id=is.xyz.mpv) - Install player from playstore then add Mi Video script in termux.
```
curl -sL "https://github.com/mmtrt/notflix-termux/raw/termux/mivideo" -o ../usr/bin/mpv && chmod +x ../usr/bin/mpv
```


## Installation

### cURL
cURL **notflix** to your **$PATH** and give execute permissions.

```
$ curl -sL "https://github.com/mmtrt/notflix-termux/raw/termux/notflix" -o ../usr/bin/notflix
$ chmod +x ../usr/bin/notflix
```
- To update, just do `curl` again, no need to `chmod` anymore.
- To uninstall, simply remove `notflix` from your **$PATH**, for example `rm -f ../usr/bin/notflix.

## License
This project is licensed under [GPL-3.0](https://raw.githubusercontent.com/Illumina/licenses/master/gpl-3.0.txt).

