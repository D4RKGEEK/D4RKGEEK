<div align="center">

<br>

# `@D4RKGEEK`

### Nine years. 55 repositories. Two public registries.

**Every claim on this page ships with the command that proves it.**

<br>

[![PyPI](https://img.shields.io/pypi/v/blare?style=for-the-badge&logo=pypi&logoColor=white&label=pypi&color=306998)](https://pypi.org/project/blare/)
[![PyPI downloads](https://img.shields.io/pypi/dm/blare?style=for-the-badge&label=installs%2Fmonth&color=2b6cb0)](https://pypistats.org/packages/blare)
[![npm](https://img.shields.io/npm/v/%40geekvb%2Fblare?style=for-the-badge&logo=npm&logoColor=white&label=npm&color=cb3837)](https://www.npmjs.com/package/@geekvb/blare)
[![Python](https://img.shields.io/pypi/pyversions/blare?style=for-the-badge&logo=python&logoColor=white&color=444)](https://pypi.org/project/blare/)
[![Runtime deps](https://img.shields.io/badge/runtime%20dependencies-0-brightgreen?style=for-the-badge)](#claims-and-how-to-check-them)

<br>

</div>

---

## Claims, and how to check them

Most profiles ask you to take their word for it. Open a terminal instead.

<table>
<tr>
<th align="center">#</th>
<th align="left">What I claim</th>
<th align="left">Run this</th>
<th align="left">What you should see</th>
</tr>

<tr>
<td align="center"><b>01</b></td>
<td>A library that sits in your production path has no business dragging a dependency tree in with it. Mine doesn't.</td>
<td><code>npm view @geekvb/blare dependencies</code></td>
<td>Nothing. Empty output. Zero runtime dependencies.</td>
</tr>

<tr>
<td align="center"><b>02</b></td>
<td>Same discipline on the Python side — not "few", none.</td>
<td><code>pip download blare --no-deps -d . && ls</code></td>
<td>One wheel. Pure Python, no C extension to compile.</td>
</tr>

<tr>
<td align="center"><b>03</b></td>
<td>The same library exists in two languages and behaves <i>identically</i>, because the spec was written before either one.</td>
<td><code>gh api repos/D4RKGEEK/blare/contents/conformance --jq '.[].name'</code></td>
<td>6 vector files. <b>90 cases.</b> Both runtimes have to pass all 90 or the build fails.</td>
</tr>

<tr>
<td align="center"><b>04</b></td>
<td>People install it without being asked to. Live number, not a screenshot from a good week.</td>
<td><code>curl -s https://pypistats.org/api/packages/blare/recent</code></td>
<td>Whatever is true today — same figure the badge above reads from.</td>
</tr>

<tr>
<td align="center"><b>05</b></td>
<td>Fire the same exception 500 times and you get <b>one</b> alert. That is the entire point, and the thing most alerting tools get wrong.</td>
<td><code>curl -sL https://raw.githubusercontent.com/D4RKGEEK/blare/main/conformance/dedupe.json | jq '.cases | length'</code></td>
<td>10 vectors that fail loudly the moment it ever double-fires.</td>
</tr>

<tr>
<td align="center"><b>06</b></td>
<td>It is finished, not "working on my machine": spec, licence, CI, and a demo a stranger runs in under a minute.</td>
<td><a href="https://d4rkgeek.github.io/blare/">d4rkgeek.github.io/blare</a></td>
<td>A live demo, <a href="https://github.com/D4RKGEEK/blare/blob/main/SPEC.md">a 30-section spec</a>, Apache-2.0.</td>
</tr>

</table>

> **If any row above is wrong, open an issue titled `claim 0X is wrong`.**
> I will either fix the code or delete the claim. Those are the only two options,
> and that is the whole method on one line.

---

## The one diagram that explains how I work

```
                        ┌───────────────────────┐
                        │       SPEC.md         │   written first, 30 sections
                        │  behaviour, in prose  │   before a line of either impl
                        └───────────┬───────────┘
                                    │
                   ┌────────────────┴────────────────┐
                   ▼                                 ▼
        ┌─────────────────────┐           ┌─────────────────────┐
        │   python/   impl    │           │    node/    impl    │
        │   0 runtime deps    │           │   0 runtime deps    │
        └──────────┬──────────┘           └──────────┬──────────┘
                   │                                 │
                   └────────────────┬────────────────┘
                                    ▼
                   ┌─────────────────────────────────┐
                   │  conformance/ · 90 vectors      │
                   │  one answer key, two runtimes   │
                   │  disagree once → red build      │
                   └─────────────────────────────────┘
```

Two implementations with one name is a trap: they drift, and your users find
out before you do. A written spec plus a shared answer key is the only version
of "cross-language" I'm willing to ship.

---

## Public, installable, today

| | | |
|:--|:--|:--|
| **Error alerting, Python + Node** | one alert instead of five hundred · spec-driven · zero deps | `Apache-2.0` · [PyPI](https://pypi.org/project/blare/) · [npm](https://www.npmjs.com/package/@geekvb/blare) · [demo](https://d4rkgeek.github.io/blare/) |
| **Music-reactive lighting engine** | reads the beat, the bars and the drops — not the volume · zero deps | `MIT` · [repo](https://github.com/D4RKGEEK/tempolight) |
| **Market-data stack** | scraper → API → frontend, four repos, messy public filings made queryable | [scraper](https://github.com/D4RKGEEK/IPOScraper) · [api](https://github.com/D4RKGEEK/IPOBackend) · [web](https://github.com/D4RKGEEK/IPOHut) · [data](https://github.com/D4RKGEEK/market_data) |

Everything above is public because it's finished. The rest of the 55 isn't.

---

## Where it runs

Not a logo wall — these are the ones I hold a bill for and debug at 2am.

**Edge & storage** &nbsp;`Cloudflare Workers` `R2` `DNS` &nbsp;·&nbsp; **Database** &nbsp;`Postgres` `Neon` `Redis` `MongoDB`
**Deploy** &nbsp;`Vercel` `Docker` `GitHub Actions` &nbsp;·&nbsp; **Metal** &nbsp;`Linux` `Raspberry Pi` `single-board targets`
**Registries** &nbsp;`PyPI` `npm` &nbsp;·&nbsp; **Languages** &nbsp;`Python` `TypeScript` `Rust` `Kotlin` `C++` `SQL`

**Problems, rather than tools:** real-time render loops and latency budgets ·
FFT, onset detection, tempo and phase tracking · error dedup and alert fatigue ·
perceptual colour in linear light · agents measured against ground truth instead
of demoed · scraping sources that actively don't want to be scraped.

---

## Currently

Two unpublished. One compiled, one not. Both held back by the same rule the rest
of this page is built on: **it goes public when it passes its own tests, and not
one day earlier.** No teasers, no roadmap, no screenshots of a localhost tab.

When they're ready, they'll show up in the table above with their own commands
to check — and you can try to break those claims too.

---

<div align="center">

<img height="160" src="https://github-readme-stats.vercel.app/api?username=D4RKGEEK&show_icons=true&hide_title=true&hide=issues&count_private=true&include_all_commits=true&theme=github_dark&hide_border=true&bg_color=0D1117&icon_color=58A6FF&text_color=C9D1D9" alt="" />
<img height="160" src="https://streak-stats.demolab.com?user=D4RKGEEK&theme=github-dark-blue&hide_border=true&background=0D1117&stroke=21262D&ring=58A6FF&fire=F78166&currStreakLabel=58A6FF" alt="" />

<br><br>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=D4RKGEEK&theme=react-dark&bg_color=0D1117&color=C9D1D9&line=58A6FF&point=F78166&area=true&hide_border=true" alt="" />

<br><br>

<picture>
  <source media="(prefers-color-scheme: dark)"
          srcset="https://raw.githubusercontent.com/D4RKGEEK/D4RKGEEK/output/github-snake-dark.svg">
  <source media="(prefers-color-scheme: light)"
          srcset="https://raw.githubusercontent.com/D4RKGEEK/D4RKGEEK/output/github-snake.svg">
  <img alt="" src="https://raw.githubusercontent.com/D4RKGEEK/D4RKGEEK/output/github-snake.svg">
</picture>

<br><br>

[![Spotify](https://spotify-github-profile.kittinanx.com/api/view?uid=31ildgflgg2mo7k6otuxlfr257ua&cover_image=true&theme=default&show_offline=false&background_color=121212&interchange=false&profanity=false&hide_remaster=false)](https://github.com/kittinan/spotify-github-profile)

<br>

**No name, no email, no hire-me banner.**
If six verifiable claims don't convince you, a bio wasn't going to.

</div>
