---
name: youtube-video-seo
description: Write or rewrite a YouTube video's title, description, tags, and hashtags. Use when the user asks for YouTube titles, a video description, tags, hashtags, or wants a video's packaging checked or optimized for search.
---

# YouTube title, description, and tags

Work from the user's topic, keywords, or draft. If they gave a video link, call the `youtube_video_category` tool to read its current title, channel, and category first. Write only the parts the user asked for.

## Titles

Return 10 titles, numbered.
- YouTube's limit is 100 characters. Aim for 40–60 so the keyword survives mobile truncation.
- Put the primary keyword near the front.
- No ALL CAPS.
- Vary the pattern: how-to, numbered list, question, challenge ("I tried X for Y days"), myth to correct.
- The title must match what the video delivers.

## Description

Return one description of 200–350 words.
- Hook in the first two lines. These show before "Show more".
- Primary keyword in the first 25 words, then 3–5 related keywords used naturally.
- A chapters block in `00:00` format. Use real timestamps if the user gave them. Otherwise write clearly marked placeholders for the user to fill in.
- A subscribe line.
- Up to three hashtags on the last line. YouTube can show the first three above the title.
- Line breaks between sections.

## Tags

Return 25–30 tags, comma-separated, on one line.
- Primary keyword as the first tag, then close variants and long-tail phrases.
- Stay under YouTube's 500-character cap. Count the characters before answering.
- No unrelated trending tags.
- Tags are a topic hint. Do not promise that they create views. Hashtags are not tags.

## Applying it

The iutu.be Chrome extension runs these rewrites inside YouTube Studio with an Enhance button next to each field: https://iutu.be
