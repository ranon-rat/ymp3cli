<h1>A simple tool to download music from youtube/spotify and listen in the terminal.</h1>

<h1>Prerequisites</h1>

- golang 1.17+
- python 3.6.1 or above (for spotdl)
- ffmpeg 4.2 or above (added to PATH)
- spotDL https://github.com/spotDL/spotify-downloader#installation

### Installing FFmpeg

- [Windows Tutorial](https://windowsloop.com/install-ffmpeg-windows-10/)
- OSX - `brew install ffmpeg`
- Linux - `sudo apt install ffmpeg`

<h1>Install instructions</h1>

- You can download the binary file from:  https://github.com/paij0se/ymp3cli/releases

- Or with curl
```bash
curl https://raw.githubusercontent.com/paij0se/ymp3cli/main/install.sh | bash
```

- verify the installation with
```bash
$ ymp3cli --h

  Usage: ymp3cli --[OPTION]
  --h,--help: Display the help command
  --v,--version: Display the version of ymp3cli

  Usage: ymp3cli [SONG]
  ymp3cli <song.mp3>: play a single song
  example: ymp3cli music/song.mp3

  Usage: ymp3cli [Link]
  ymp3cli <link>: download a song from youtube
  example: ymp3cli https://www.youtube.com/watch?v=dQw4w9WgXcQ

	 MIT License
	 Made it by pai
	 https://paijose.cf


$ ymp3cli # start ymp3cli

$ ymp3cli https://www.youtube.com/watch?v=dQw4w9WgXcQ # download a song from youtube

$ ymp3cli song.mp3 # play a single song

```

<h1>Build instructions</h1>

for linux install the oto dependencies

```bash
sudo apt install libasound2-dev
```
for macOS Oto requies `AudioToolbox.framework`, but this is automatically linked.

run `go get .` to install the dependencies.

Build ymp3cli with `go build -o ymp3cli src/main.go`

and for execute ymp3cli just run `./ymp3cli`.


<div align=center>

<img src="https://you-can.ml/monda/yessir.gif"/>

<h1>Discord RPC</h1>

<img src="https://cdn.discordapp.com/attachments/786759600245309460/922690903750086796/Screenshot_from_2021-12-20_22-23-45.png"/>
</div>

<h1>TODO:</h1>

- [x] client in golang
- [x] download the videos without youtube-dl
- [x] works correctly in windows
- [x] Discord rpc
- [ ] able to pause and rewind the songs
- [ ] A playlists system
- [x] able to play a song one by one

<h1>Custom clients?</h1>
- visit the wiki https://github.com/paij0se/ymp3cli/wiki/Routes

<h1>Alternative clients</h1>
- The old deno client https://github.com/bruh-boys/ymp3cli-old-client

<h1>Thanks to</h1>
- Flames https://github.com/FlamesX-128
