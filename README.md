<div align="center">

### @D4RKGEEK

**Writing software since 2017.**

Nine years of it. Published libraries, real-time systems, data pipelines,
and a few things still running on other people's machines.

I don't write about what I'm building until it's finished,
so this page is about *how* I build rather than what.

</div>

---

## What I've actually worked in

| | |
|---|---|
| **Real-time systems** | 60 fps render loops, UDP streaming, latency budgets, no-allocation hot paths |
| **Audio DSP** | FFT, spectral flux, onset detection and classification, tempo and phase tracking |
| **Observability** | error capture, deduplication, alert fatigue, cross-language conformance |
| **Data extraction** | scraping messy public sources into something queryable |
| **Colour science** | OkLab and OkLch, perceptual gradients, working in linear light |
| **LLM systems** | agents measured against ground truth rather than demoed |
| **Shipping** | packages on PyPI and npm, Docker, CI, Linux and single-board targets |

`Python` `TypeScript` `Rust` `Kotlin` `C++` `SQL` — plus whatever the problem
turns out to need.

---

## How I work

**I measure the thing I claim.** Not "it feels synced" but the phase error in
beats. Not "onsets are detected" but 5.28 a second measured against the 1.07
actually in the track. A test proving only that the output is finite and in
range will pass happily while the thing renders solid black — that has caught
me four separate times, so now I render it and look.

**Zero dependencies, where it matters.** The FFT, the JSON parser, the HTTP
server, the colour maths — hand-written, more than once. A binary under a
megabyte that runs on a Pi Zero is worth more than the afternoon a library
would have saved. A package that sits in someone else's production path has no
business dragging a tree in with it.

**One spec, two implementations, one behaviour.** When the same library has to
exist in two languages, the spec is written down first and a conformance suite
proves both sides agree. Otherwise you've shipped two subtly different products
with one name.

**Finished means documented.** A spec, a licence, CI, and a demo a stranger can
run in under a minute. Otherwise it isn't done — it's working on my machine.

**I'd rather be corrected than agreed with.** The last thing I was confident and
wrong about was a colour-space assumption that didn't survive being measured.
Finding that out cost a week and taught me more than the month before it.

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

</div>
