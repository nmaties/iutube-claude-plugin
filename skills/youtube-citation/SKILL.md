---
name: youtube-citation
description: Cite a YouTube video in APA 7, MLA 9, Chicago 17, or Harvard style, with the in-text citation. Use when the user asks how to cite or reference a YouTube video.
---

# Cite a YouTube video

## Fields

- Channel name
- Video title
- Upload date
- URL
- Date accessed (MLA optional, Harvard required)
- Video length (Chicago, optional)

If the user gave a link, call the `youtube_video_category` tool to read the title, channel, and duration. The tool does not return the upload date. Ask the user for it. Never guess a date. If a field is still missing, leave its placeholder in the citation (for example `Year, Month Day`) and say which field to fill in.

## Formats

Titles shown in *italics* below are italic in the citation. Return the style the user asked for, or all four if they named none.

**APA 7**
- Reference: Channel name. (Year, Month Day). *Title of video* [Video]. YouTube. https://www.youtube.com/watch?v=…
- In-text: (Channel name, Year)

**MLA 9**
- Reference: “Title of video.” *YouTube*, uploaded by Channel name, Day Mon. Year, www.youtube.com/watch?v=…. Accessed Day Mon. Year.
- In-text: (“Title of video”)
- Drop `https://` from the URL. Month abbreviations: Jan., Feb., Mar., Apr., May, June, July, Aug., Sept., Oct., Nov., Dec. Leave out the Accessed sentence if there is no access date.

**Chicago 17**
- Bibliography: Channel name. “Title of video.” Month Day, Year. YouTube video, 12:34. https://www.youtube.com/watch?v=….
- Footnote: Channel name, “Title of video,” Month Day, Year, YouTube video, 12:34, https://www.youtube.com/watch?v=….
- Leave out the length if it is unknown.

**Harvard**
- Reference: Channel name (Year) *Title of video*. Day Month. Available at: https://www.youtube.com/watch?v=… (Accessed: Day Month Year).
- In-text: (Channel name, Year)

Harvard varies by institution. Tell the user to check their own style guide.

Web version: https://iutu.be/how-to-cite-a-youtube-video
