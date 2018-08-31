bbc_radio.sh
============

A simple bash script to play BBC Radio at the terminal.  Supports the following stations (options):

1. BBC Radio One (**radio_one**)
2. BBC Radio Two (**radio_two**)
3. BBC Radio Three (**radio_three**)
4. BBC Radio Four (**radio_fourfm**)
5. BBC Radio Five Live (**radio_five_live**)
6. BBC Radio 6 Music (**6music**)

The script will first try to play using _mpc_, failing that, _mplayer_.  For example, to play Radio One with mplayer, the URL would look like:

```console
mplayer http://a.files.bbci.co.uk/media/live/manifesto/audio/simulcast/hls/uk/sbr_high/ak/bbc_radio_one.m3u8
```

Or Radio Four using _mpc_:

```console
mpc http://a.files.bbci.co.uk/media/live/manifesto/audio/simulcast/hls/uk/sbr_high/ak/bbc_radio_fourfm.m3u8
```

Setup
-----

To get setup, clone the git repository and make sure the file is executable.

```console
cd ~
git clone https://github.com/crazzyfool/bbc_radio.sh.git
cd ~/bbc_radio.sh
```

Make sure the script is executable.

```console
chmod -v u+x ~/bbc_radio.sh/bbc_radio.sh
```

Usage
-----

To use, simply either run without any options and select a station.

```console
cd ~/bbc_radio.sh
./bbc_radio.sh
```

Or run with a station as an option.

```console
./bbc_radio.sh radio_one
```
