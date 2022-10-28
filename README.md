# discord-music
<div align='center'>
<a><strong>Simply Discord Music</strong></a>
<p>
    <a href="https://github.com/brokenedtz/discord-music/actions" target="_blank"><img alt="GitHub Workflow Status" src="https://img.shields.io/github/workflow/status/brokenedtzjs/discord-music/Testing?label=Tests&logo=github&style=flat-square"></a>
    <br>
    <a href="https://github.com/brokenedtzjs/discord-music/stargazers" target="_blank"><img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/brokenedtzjs/discord-music?logo=github&logoColor=white&style=flat-square"></a>
  </p>
</div>
</div>

## Installation

```npm
$ npm install @brokenedtzjs/discord-music@latest
```

Or add this package to your `package.json` file:

```json
"dependencies": {
    "@codertocat/hello-world-npm": "1.0.0"
}
```

## Requirements
- Node.js 16.9.0 or higher
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
music.on('playing', (queue, music) => {
  //code
)};
```
