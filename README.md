# iutu.be YouTube tools for Claude

YouTube creator tools from [iutu.be](https://iutu.be) for Claude. Ask Claude how long a playlist is, what category a video is in, or for titles, descriptions, tags, opening hooks, channel names, video ideas, citations, and earnings estimates. No sign-in and no API key.

This plugin is made by iutu.be. It is not affiliated with or endorsed by YouTube or Google.

## What it adds

MCP tools, served by `https://iutu.be/mcp` (no sign-in, no API key):

| Tool | What it does |
| --- | --- |
| `youtube_playlist_length` | Total length, video count, and every watch link of a public playlist (first 300 videos) |
| `youtube_video_category` | Category, title, channel, and duration of a public video |

Skills:

| Skill | What it does |
| --- | --- |
| `youtube-playlist-and-category` | Runs the two lookups above and reports the result |
| `youtube-video-seo` | 10 titles, a description, and tags for a video |
| `youtube-intro-hooks` | 10 spoken opening lines for the first 5–10 seconds |
| `youtube-channel-names` | 20 channel names for a niche |
| `youtube-video-ideas` | 12 video ideas for a niche, two of them Shorts |
| `youtube-citation` | APA 7, MLA 9, Chicago 17, and Harvard citations |
| `youtube-earnings` | Earnings estimate from views and RPM |

Claude loads a skill when a request matches it. You can also call one directly, for example `/iutube:youtube-intro-hooks How I built a desk for $40`.

Exporting YouTube subscriptions needs a Google sign-in, so it stays on the site: https://iutu.be/export-youtube-subscriptions

## Install

In Claude Code:

```
/plugin marketplace add nmaties/iutube-claude-plugin
/plugin install iutube@iutube
```

From a local checkout of this repository:

```bash
claude --plugin-dir .
```

## What the plugin sends

The plugin runs no code on your machine. It has no hooks and no scripts.

The two MCP tools send the playlist or video link you give them to `https://iutu.be/mcp`. That server reads the public YouTube page and returns the result. It needs no account, and the plugin sends nothing else. The skills are instructions for Claude and make no network requests of their own.

Privacy policy: https://iutu.be/privacy-policy

## License

MIT. See [LICENSE](LICENSE).
