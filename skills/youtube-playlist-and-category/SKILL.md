---
name: youtube-playlist-and-category
description: Look up a public YouTube playlist's total length, video count, and watch links, or a public video's YouTube category. Use when the user asks how long a playlist is, wants every link in a playlist, or asks what category a video is in.
---

# YouTube playlist length and video category

Both lookups run on the iutu.be MCP server bundled with this plugin. They read public YouTube pages. No sign-in and no API key.

## Playlist length and links

Call the `youtube_playlist_length` tool with `url` set to the playlist URL (`youtube.com/playlist?list=…`) or the playlist id.

Report:
- the playlist title, total length, and video count
- if `truncated` is true, that only the first 300 videos were read
- if `missingDurationCount` is above 0, how many videos had no duration and are left out of the total
- the watch links, when the user asked for them. For a long playlist, offer the list instead of printing all of it unasked.

If the user asks for the length at another playback speed, divide `totalSeconds` by the speed.

## Video category

Call the `youtube_video_category` tool with `url` set to a watch URL, a Shorts URL, a youtu.be link, or an 11-character video id. Report the category, title, channel, and duration.

## Errors

- Private or deleted playlists and videos cannot be read. Ask for a public link.
- YouTube sometimes asks the server to sign in for a public video, and the tool reports it as private or blocked. If the user says the video is public, say the lookup failed for that video and do not claim it is private.
- The server limits lookups to 12 playlists and 20 videos per 10 minutes. If the limit message comes back, tell the user to wait a few minutes. Do not retry in a loop.

Web versions: https://iutu.be/youtube-playlist-length-calculator and https://iutu.be/youtube-category-checker
