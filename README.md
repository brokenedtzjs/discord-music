<div align='center'>

[![Visitors](https://visitor-badge.glitch.me/badge?page_id=brokenedtzjs.discord-music)](https://github.com/brokenedtzjs/discord-music)
[![Discord](https://img.shields.io/discord/984857299858382908)](https://discord.gg/YyzghaDU9C)
[![Stars](https://img.shields.io/github/stars/brokenedtzjs/discord-music?logo=github)](https://github.com/brokenedtzjs/discord-music)
[![Issues](https://img.shields.io/github/issues/brokenedtzjs/discord-music)](https://github.com/brokenedtzjs/discord-music/issues)
[![Twitter](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Ftwitter.com%2Fcyrabot)](https://twitter.com/cyrabot)

</div>

# discord-music
Simply Discord Music  

## Features

- Based on
- [@discordjs/voice](https://github.com/discordjs/voice)
- [DisTube](https://github.com/skick1234/DisTube)
- [@distube/ytdl-core](https://github.com/skick1234/DisTube)
- [@distube/ytpl](https://github.com/skick1234/DisTube)
- [@distube/ytsr](https://github.com/skick1234/DisTube)
- Easy to use and customize
- Support YouTube and audio link
- Audio filters (bassboost, nightcore, vaporwave, and more)
- Autoplay related songs

## Installation

```npm
$ npm install @brokenedtzjs/discord-music@latest
```

## Requirements
- [Node.js](https://nodejs.org) 16.9.0 or higher
- [discord.js](https://discord.js.org) v13
- [@discordjs/voice](https://github.com/discordjs/voice)
- [FFmpeg](https://www.ffmpeg.org/download.html)
- [@discordjs/opus](https://github.com/discordjs/opus)
- [sodium](https://www.npmjs.com/package/sodium) or [libsodium-wrappers](https://www.npmjs.com/package/libsodium-wrappers)

## Quick Start
```js
const DiscordMusic = require('@brokenedtzjs/discord-music');
const music = new DiscordMusic(client, {
  //code
});
module.exports = music;
```

```js
music.on('playing', (queue, song) => {
  //code
});
```

## Example
```js
const DiscordMusic = require('@brokenedtzjs/discord-music');
const music = new DiscordMusic(client, {
  LeaveIfEmpty: true, //true = if channel is empty bot will leave the channel
  LeaveIfFinish: true, //true = if song played finish bot will leave the channel
  LeaveCooldown: 3, //seconds (leave cooldown)
});
```

## Playing

```js
music.on('playing', (queue, song) => {
  queue.VoiceChannel.send(`Playing ${song.name} | ${song.duration}`); //send message when music start playing
});
```

## AddSong

```js
music.on('addSong', (queue, song) => {
  queue.VoiceChannel.send(`Queue Added ${song.name} | ${song.duration}`); //send message when added song to queue
});
```

glpat-G6hEN3mTpGcyJDpywYvv

40616718