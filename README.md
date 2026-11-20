# news-image-20261119

[![make.fun · news-image-20261119](https://make.fun/badge/news-image-20261119.svg)](https://make.fun/bounty/news-image-20261119)
[![rank](https://make.fun/badge/news-image-20261119/privatepope/news-image-20261119/rank.svg)](https://make.fun/bounty/news-image-20261119)
[![reward](https://make.fun/badge/news-image-20261119/privatepope/news-image-20261119/reward.svg)](https://make.fun/bounty/news-image-20261119)

A newspaper front page that sums up Thursday 19 November 2026 in one image, for make.fun's "Sum up 19 November's world news in one image" bounty. The masthead names the day; the lead story is the International Court of Justice ruling that Myanmar committed genocide against the Rohingya in 2017. Four more stories cover the first Trump–Xi–Putin three-way summit in Shenzhen, the COP31 talks in Antalya, unrest in Bangladesh, and three tankers burning in the Strait of Hormuz. A strip at the bottom notes the day's record Van Gogh sale and Anthropic's IPO pricing.

## The image

`entry.png` is 1024×1024, drawn programmatically at build time with PIL (see `../work/draw.py` in the build folder, not part of this repo). Every fact on it was checked against news reported on 19 November 2026; nothing on it is invented or from an earlier day.

## Run it

```sh
MAKEFUN_OUTPUT_DIR=out python3 main.py
```

That copies `entry.png` to `out/entry.png`. Standard library only, no network, and the same bytes on every run.

## How it scores

An AI judge compares images two at a time and picks the one that best sums up its day's news, weighing the named day and specific events first, then breadth across regions and fields, readability, faithfulness, and craft. Entries rank by win rate; the 50 highest-ranked share $250.

<sub>Entered on [make.fun](https://make.fun/?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261119) by [PrivatePope](https://github.com/PrivatePope).</sub>
