# YouTube Home filters for Brave

Custom cosmetic filters for the YouTube website in Brave. Mobile and desktop lists are separate.

| Version | Website | Filter subscription URL |
| --- | --- | --- |
| Mobile | `m.youtube.com` | [Mobile filter](https://raw.githubusercontent.com/donatopellegrino/youtube-filters/main/duration-filter-grey.txt) |
| Desktop | `www.youtube.com` | [Desktop filter](https://raw.githubusercontent.com/donatopellegrino/youtube-filters/main/duration-filter-desktop-grey.txt) |

## Install

1. Open `brave://settings/shields/filters` in Brave. On Android, you can also open Settings → Brave Shields & privacy → Content filtering.
2. Under **Add custom filter lists**, paste the appropriate raw subscription URL from the table and add it.
3. Remove older manually pasted versions of these YouTube rules, then reload YouTube.

After a repository update, use **Update now** in Brave's filter-list settings and reload YouTube to fetch the latest version without waiting for a background update.

## Behavior

On Home, regular videos shorter than 15 minutes retain their space and duration badge, but their thumbnail and channel avatar become grey, their title becomes `REDACTED`, their channel name and statistics are removed, and clicking is disabled. Videos of 15 minutes or longer retain their cards' normal behavior.

All Home video previews are visually suppressed, including previews of longer videos. Watch-page playback is unaffected. Search and channel pages are outside the intended filter scope. These lists add no Shorts filtering; manage Shorts separately in Brave.

The rules match English duration labels. They depend on YouTube's page markup and may need updates when YouTube changes its website. Cosmetic filtering does not guarantee that video or preview data will not be downloaded.
