# <img src='https://raw.githack.com/FortAwesome/Font-Awesome/master/svgs/solid/music.svg' card_color='#010101' width='50' height='50' style='vertical-align:bottom'/> Jellyfin
This skill is a fork of the emby skill that allows audio playback from a Jellyfin server. Now this repo is owned by Lost Light Projects.

## About
Stream music from your Jellyfin server using Mycroft! Play all songs by an artist or an instant mix of any artist/album/song in your Jellyfin library.

This has been tested on Zorin OS 16 (Ubuntu 20.04 LTS) using VLC audio backend and PiCroft using Google AIY Voicekit and VLC


## Examples

## Credits
rickyphewitt (Emby)

## Category
**Music**

## Tags
#Jellyfin,#Music


## Community
I now have a Matrix Chat setup #mycroft-jellyfin-skill:matrix.org
Note: I have not yet setup a bridge to telegram. It is on a to-do list.

## Bugs
* Common Play Framework not working with anything except "pause, next song, stop, resume"
* I can't seem to get it to play a specific song

## Fixed Issues
* Playlists now play
* Settings in home.mycroft.ai fixed (wasn't showing up)

## Installation
* mycroft-msm install https://github.com/LostLightProjects/jellyfin-skill/

## Picroft
You will need to install vlc, installing just vlc-bin will not work which is really annoying.
This requirement might change as mycroft supports more audio backends.
* sudo apt update && sudo apt upgrade
* sudo apt install vlc

The common play framework does not work on picroft at the moment as the queries timeout before the request is complete, this is a bug in the playback control skill so for now you will have to use the "from jellyfin" intent, eg; "Play artist Blackmore's Night from jellyfin"

## Common Play Framework
This skill supports the common play framework! This means you don't have to specify "Jellyfin" in your intent. For Example
* "Play The Beatles"
* "Play artist The Beatles"
* "Play playlist fun mix"
* "Play song Hey Jude"
* "Play heavy metal"
* "next song"
* "pause"
* "stop"
* "resume"

## From Intent
If you have other music services you can use the from intent
* "Play artist Blackmore's Night from jellyfin"
* "Play playlist fun mix from jellyfin"
* "Play rock from jellyfin"

## OTHER Features
You can ask for the track information.
* "what song is this"

You can shuffle your music
* "shuffle"

You can add the currently playing song to a playlist(it has to exist)
* "add to (playlist name)"
* "add to fun mix"

## Set up
Go to https://account.mycroft.ai/skills
Make sure to enter in your jellyfin server URL and login credentials.

## Contributing
Always looking for bug fixes, features, translation, and feedback that make the Jellyfin for Mycroft experience better!

## Troubleshooting
### Setup Connection Info
* Ensure your host, port, username, and password are set at https://account.mycroft.ai/skills
### Check Server Connection
* "Check Jellyfin/Emby"
* This will attempt to connect then authenticate to your Jellyfin server using the connection info provided above


