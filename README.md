# Nightcore Maker

[![Build](https://github.com/NetherMCtv/nightcore-maker/actions/workflows/build.yml/badge.svg)](https://github.com/NetherMCtv/nightcore-maker/actions/workflows/build.yml)

A Node.js program to make a nightcore version of a music in 10 seconds

## How it works

* Asks for a YouTube video URL and download its audio
* Grabs a random wallpaper using the [r/AnimeWallpaper](https://www.reddit.com/r/AnimeWallpaper) subreddit (filter by top posts and only desktop wallpapers) and downloads it [[Why did I take a subreddit for the wallpaper?](#why-did-i-take-a-subreddit-for-the-wallpaper)]
* Using the downloaded audio, FFmpeg will speed it up 0.25x faster
* Now that we have the faster audio (the nightcore version) and the wallpaper, we need the merge them to make a video [Not done yet]

## Using it

Download Nightcore Maker with the [latest release](https://github.com/NetherMCtv/nightcore-maker/releases/latest) and [FFmpeg](https://ffmpeg.org/download.html), then in a command prompt (cmd/bash), run:

```bash
./file-you-ve-downloaded <video-url>
```

### Options

```bash
Usage: nightcore-maker [options] <video>

A Node.js program to make a nightcore version of a music in 10 seconds 

Arguments:
  video                Video URL

Options:
  -V, --version        output the version number
  -s, --speed <speed>  speed of the new audio (default: 1.25)
  -f, --fps <fps>      fps of the video (default: 25)
  -h, --help           display help for command
```

## Todo

- [ ] Add download and audio/video generation progress bars
- [ ] Uploading to YouTube
- [x] Replace `config.ini` by CLI options 

## Notes

### Why did I take a subreddit for the wallpaper?

I've search for 3h+ for an API for random anime wallpaper, I know Pixiv but this is nightmare for logging in. 1h30-2h of research, which didn't really help me because I couldn't connect to use their API... 😐

Finally took the subreddit because I've had enough of these login problems