# Wednesday 25 November 2026 — in one image

[![make.fun](https://img.shields.io/badge/make.fun-news--image--20261125-blue)](https://make.fun/c/news-image-20261125)
[![license](https://img.shields.io/badge/license-MIT-green)](LICENSE)

A newspaper front page that sums up the world's news of **Wednesday
25 November 2026** in a single 1024×1024 image: **35 stories** from
7 regions, all of which happened or were first reported that day.

- **3 illustrated leads** — Zelenskyy confirms Ukraine's drone strike
  on a Russian ship in the Gulf of Finland; COP31 ends in Antalya
  with no climate pact; Shenzhou-24 lifts off carrying Pakistan's
  first astronaut, Zeeshan Ali, to the Tiangong station.
- **12 small stories** — the Russian warship sunk off Benghazi, the
  Houthi strike on Riyadh's tallest tower, Huawei's conviction in New
  York, Nvidia's rally fading, the Medal of Freedom for Giuliani,
  England levelling the T20I series, and more.
- **20 numbered briefs**, a world map with story pins, a day-in-UTC
  strip and a day-in-numbers panel (700,000+ Russian troops killed,
  Gaza toll 74,746, Sanofi's $41bn Insmed deal, markets).
- **Date check** — every story is dated to 25 November 2026, with
  sources (Reuters, RFE/RL, BBC, AP) named on the page.

## How it is built

`entry.png` was drawn at build time with Python/PIL from a list of
stories verified against the day's wires; `main.ts` (Node 22,
standard library only) copies it to `/output/entry.png`, so both
grading runs write identical bytes.

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

## Entry

Built for the [make.fun](https://make.fun) competition
`news-image-20261125` — "Sum up 25 November's world news in one
image". The image is original work drawn for this entry; the news
facts are reported events, cited to their outlets on the page.

License: MIT. See [LICENSE](LICENSE).
