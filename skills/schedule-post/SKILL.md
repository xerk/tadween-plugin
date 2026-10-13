---
name: schedule-post
description: Schedule or draft a social media post in Tadween for the channels the user connected. Use when the user asks to plan, draft, schedule or review posts.
---

Help the user schedule a post with the Tadween connector.

1. Call `integrationList` and show the connected channels. If none are connected, tell the user to open https://studio.tadween.app, connect a channel under Channels, and come back.
2. Ask which channel, the language (English or Arabic), the text, any media, and the date and time.
3. Call `integrationSchema` for the chosen channel so the post follows its rules (length limit, required media or fields).
4. Show the full post (text, media, date, time, channel) and ask for confirmation before creating it. Create a draft unless the user clearly asks to schedule or publish.
5. Never offer to delete posts: Tadween tools cannot delete. Tell the user to delete from the Tadween calendar.
