# Bishops Chamblee: Instagram image drop

This repo is public so Instagram can fetch images from it. Only put images here that are meant to be posted.

## How it works

1. Drop the image into `to-post/`.
   - JPEG is best. PNG is fine too; it gets converted to JPEG before posting.
   - Under 8 MB, and between 4:5 (portrait, 1080x1350) and 1.91:1 (landscape). Square 1080x1080 works.
2. Optional: add a caption file with the same name, e.g. `holiday-hours.jpg` + `holiday-hours.txt`.
   No caption file? Ask Claude to write one, or give it in the chat.
3. Tell Claude in the Bishops Campaigns project what to post and when ("post holiday-hours today at noon").
4. After it's posted, Claude moves the image (and caption) to `posted/<date>/`.

Posts go to @bishops.chamblee through the Windsor.ai connector. Windsor posts right away, so a scheduled post is Claude coming back at the set time and posting it then.

## Folders

- `to-post/`: waiting to be posted
- `posted/`: already on Instagram (`2026-11-reopening-week` was posted by hand in Meta Business Suite)
