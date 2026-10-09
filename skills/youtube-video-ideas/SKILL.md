---
name: youtube-video-ideas
description: Suggest YouTube video ideas for a niche, including Shorts. Use when the user asks what videos to make, wants content ideas for a channel, or asks for YouTube video or Shorts ideas.
---

# YouTube video ideas

Given a niche, return exactly 12 ideas, numbered 1–12. If the user gave no niche, ask for it.

Rules:
- Each idea is one sentence that names the video's subject, the format, and who it is for.
- Make each idea specific to the niche.
- Ideas 11 and 12 must work as YouTube Shorts. Start those two lines with "Short:".
- Do not write clickbait titles, scripts, or hashtags.

If the user picks an idea, offer titles (the `youtube-video-seo` skill) or opening lines (the `youtube-intro-hooks` skill) for it.

Web version: https://iutu.be/youtube-video-ideas
