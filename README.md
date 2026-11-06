# 📺 Bachpan TV

An old-style CRT TV on the web. Turn it on — classic Indian shows are already playing, live-TV style.
Flip the channel to change the show. That's it.

**Only 3 controls exist: Power · Channel +/− · Volume +/−.** No pause, no play, no episode list, no login.

Live site (after the GitHub push): https://ankitgarg43.github.io/bachpan-tv/

## Channels

| CH | Show | Streams from (official YouTube) | Episodes in playlist* |
|----|------|--------------------------------|-----------------------|
| 1 | Shaka Laka Boom Boom | StarPlus Classics — "Full Episodes" playlist | 73 and growing |
| 2 | Shararat – Thoda Jaadu, Thodi Nazaakat | StarPlus Classics — "Full Episodes" playlist | 125 |
| 3 | Malgudi Days | Ultra Bollywood — "Malgudi Days TV Series - Full Episodes" | 54 (complete series) |
| 4 | Shaktimaan | Ultra Kids Zone — शक्तिमान playlist | 276 |
| 5 | Son Pari | StarPlus Classics — "Full Episodes" playlist | 81 and growing |

\* StarPlus Classics is still adding episodes to its playlists, so CH 1, 2 and 5 keep growing on their own.
The TV reads the real playlist length from YouTube and corrects its schedule automatically.

## How the "live" TV works

There is no server and nothing is hosted here — every show plays through YouTube's official embed player,
straight from the rights-holder's own channel, so there are no copyright files on this site.

The episode and the position inside it are **calculated from the clock** (a fixed schedule slot per channel,
based on the median episode length of that show's playlist). So:

- Everyone who turns the TV on at the same moment lands on the same episode at about the same point.
- Leaving and coming back is like leaving a real TV on — the show has moved on without you.
- When an episode ends early or late versus its slot, the TV hops back onto the schedule.

## Controls

- **⏻ Power** — TV on / off
- **Channel + / −** — next / previous show (with static + channel display, like a real TV)
- **Volume + / −** — sound up / down (on-screen volume bar)
- Keyboard: ↑/↓ channel, ←/→ volume, `P` power

The picture itself cannot be clicked, so nobody can pause it or click away to YouTube.

## Files

- `index.html` — the whole TV (single self-contained file)
- `favicon.svg`, `manifest.webmanifest`, `robots.txt`, `sitemap.xml` — icons / SEO housekeeping
- `PUSH-TO-GITHUB.md` — 2-minute publish steps

## Note on CH 3 (Malgudi Days)

CH 3 uses Ultra Bollywood's official playlist — Ultra is the rights-holder channel for this series on YouTube
(the older Rajshri uploads are no longer live). If YouTube ever restricts embedding on that playlist,
CH 3 is the channel that would show a YouTube error; the other four are unaffected.
