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
pkg up -y && pkg in binutils fzf git nodejs python -y
```

* [webtorrent](https://webtorrent.io/) - A tool to stream torrent.
```
npm install webtorrent-cli -g
```
* [termux-open-url](https://github.com/mmtrt/notflix-nyaa-termux/raw/termux/src/termux-open-url) - Add termux-open-url script as mpv script in termux to open url with players.
```
curl -sL "https://github.com/mmtrt/notflix-nyaa-termux/raw/termux/src/termux-open-url" -o ../usr/bin/mpv && chmod +x ../usr/bin/mpv
```

## Optional

* [mpv-android](https://play.google.com/store/apps/details?id=is.xyz.mpv) - Install it from playstore then add mpv script in termux.
```
curl -sL "https://github.com/mmtrt/notflix-nyaa-termux/raw/termux/src/mpv" -o ../usr/bin/mpv && chmod +x ../usr/bin/mpv
```
* [MX Player](https://play.google.com/store/apps/details?id=com.mxtech.videoplayer.ad) - Install it from playstore then add MXPlayer script in termux.
```
curl -sL "https://github.com/mmtrt/notflix-nyaa-termux/raw/termux/src/mxplayer" -o ../usr/bin/mpv && chmod +x ../usr/bin/mpv
```
* [VLC](https://play.google.com/store/apps/details?id=org.videolan.vlc) - Install it from playstore then add VLC script in termux.
```
curl -sL "https://github.com/mmtrt/notflix-nyaa-termux/raw/termux/src/vlc" -o ../usr/bin/mpv && chmod +x ../usr/bin/mpv
```
* [Mi Video](https://play.google.com/store/apps/details?id=is.xyz.mpv) - Install it from playstore then add Mi Video script in termux.
```
curl -sL "https://github.com/mmtrt/notflix-nyaa-termux/raw/termux/src/mivideo" -o ../usr/bin/mpv && chmod +x ../usr/bin/mpv
```


## Installation

### notflix
cURL **notflix** to your **$PATH** and give execute permissions.

```
curl -sL "https://github.com/mmtrt/notflix-nyaa-termux/raw/termux/notflix" -o ../usr/bin/notflix && chmod +x ../usr/bin/notflix
```
- To update, just do `curl` again, no need to `chmod` anymore.
- To uninstall, simply remove `notflix` from your **$PATH**, for example `rm -f ../usr/bin/notflix.

### nyaa
cURL **nyaa** to your **$PATH** and give execute permissions.

```
curl -sL "https://github.com/mmtrt/notflix-nyaa-termux/raw/termux/nyaa" -o ../usr/bin/nyaa && chmod +x ../usr/bin/nyaa
```
- To update, just do `curl` again, no need to `chmod` anymore.
- To uninstall, simply remove `nyaa` from your **$PATH**, for example `rm -f ../usr/bin/nyaa.

## License
This project is licensed under [GPL-3.0](https://raw.githubusercontent.com/Illumina/licenses/master/gpl-3.0.txt).

