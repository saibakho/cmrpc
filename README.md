# cmrpc - A Discord RPC for C* Music Player

### with some more features:
- Discord RPC (Albumart as icons!!)
- notify-send when song changes

- to-dos:
	- jp2a visualizer

### About albumart

- For notifier:
	- Extract from mp3 with `ffmpeg`
	- temporarily stored in `~/.config/cmus/covers`(auto create if not exists). 
	- removed when the above directory contains more than 10 jpeg files.
	- (may be combined with the below method)

- For Discord Rich Presence Icon:
	- Discord RPC can now display images via url
	- fetched from [MusicBrainz](https://musicbrainz.org/) database (may not be found)
	- (may use images from `ffmpeg` if discord support local images :( )

### Usage

- Requirements
	- `ffmpeg`
	- `python 3.10` (match-case used) with below packages
	```bash
		pip install pypresence
		pip install musicbrainzngs
	```

- run in background with cmus
	```bash
		/path/to/cmrpc 1>/dev/null & cmus
	```


