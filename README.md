# iutu.be plugin for Claude

YouTube creator tools from [iutu.be](https://iutu.be) for Claude Code.

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
