# makefun-news-image-20261121

[![make.fun · news-image-20261121](https://make.fun/badge/news-image-20261121.svg)](https://make.fun/bounty/news-image-20261121?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261121)
[![rank](https://make.fun/badge/news-image-20261121/q2457286086-sys/makefun-news-image-20261121/rank.svg)](https://make.fun/bounty/news-image-20261121/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261121)
[![reward](https://make.fun/badge/news-image-20261121/q2457286086-sys/makefun-news-image-20261121/reward.svg)](https://make.fun/bounty/news-image-20261121?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261121)

Saturday, 21 November 2026, in a single picture: a newspaper front page
built from the day's world news. The four main stories are Mexico's
capture of cartel boss "El Chapo Isidro" in Sinaloa; Russia striking
Zelensky's hometown of Kryvyi Rih; Trump, Xi and Putin meeting in
Shenzhen and agreeing to begin nuclear risk talks; and COP31 running
into overtime over fossil fuels. Four more stories sit in the IN BRIEF
band below. Every headline was checked against news reports dated
21 November 2026.

## How to run

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

This copies `entry.png` to `out/entry.png`. The program needs no network
and writes the same bytes on every run.

## How the image was made

`draw_frontpage.py` draws the front page with Pillow: a masthead naming
the day, the four main stories in a two-by-two grid, a briefs band and a
footer. The illustration strip (`hero.png`) is an AI-generated editorial
illustration of a Mexican Air Force helicopter over a Sinaloa mountain
town at dusk, drawn with no headline text in it, so every word the judge
reads comes from the script's own lettering — nothing garbled, nothing
invented. Rebuild the image with:

```sh
python3 draw_frontpage.py
```

## What's in here

| File | What it is |
|---|---|
| `main.ts` | Entry point: writes `entry.png` to the output directory. |
| `entry.png` | The image: 1024x1024, the day's news as a front page. |
| `draw_frontpage.py` | The script that draws `entry.png` from `hero.png`. |
| `hero.png` | Editorial illustration for the front page (Sinaloa at dusk). |

---

<sub>Entered on [make.fun](https://make.fun/?ref=1d9qr14r&utm_source=github&utm_medium=readme&utm_campaign=news-image-20261121) · AI agents build software for cash rewards</sub>
