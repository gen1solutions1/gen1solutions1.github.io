# Gen1 Solutions - Reels Portfolio

Live at: https://gen1solutions1.github.io

## Add a new reel

1. Export the reel as MP4 (H.264, 1080x1920). Keep it **under 25 MB** - that is GitHub's limit for browser uploads. HandBrake (free) can shrink a 60 second reel to around 10 to 15 MB with no visible loss.
2. In this repo, click **Add file > Upload files**, drop the MP4 in, and commit. (Put it in a folder called "reels" by naming it reels/your-file.mp4, or just upload to the main folder and use the plain file name below.)
3. Open `reels.js`, click the pencil icon, and add one block inside the list:

```js
{
  title: "Your reel title",
  client: "Who it was for",
  category: "Lectures",
  file: "reels/your-file-name.mp4"
},
```

4. Commit. The site updates in about a minute.

Newest first? Just paste the new block at the top of the list.

## Bigger videos

For anything over 25 MB, upload it to YouTube (unlisted is fine) and use `youtube: "VIDEO_ID"` instead of `file`. Example in `reels.js`.

## First things to change in reels.js

- `whatsapp` - your number with country code, no + (e.g. 923001234567)
- `email` - your email

The WhatsApp and email buttons stay hidden until these are filled in.

## Good to know

- Keep the whole repo under 1 GB. That is roughly 60 to 80 compressed reels. After that, move older ones to YouTube.
- Categories (filter buttons) are created automatically from the `category` field.
- Want it on your own domain later, like portfolio.gen1sol.com? Settings > Pages > Custom domain.
