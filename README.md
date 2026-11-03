<div align="center">

# Vaibhav

**Building since 2017.**

Error alerting that doesn't spam you. Market data pipelines.
A lighting engine that hears the beat. An AI that fixes real bugs.

Small tools, finished properly, with claims I can measure.

[blare](https://github.com/D4RKGEEK/blare) ·
[Tempolight](https://github.com/D4RKGEEK/tempolight) ·
[getmendloop@gmail.com](mailto:getmendloop@gmail.com)

</div>

---

## What I'm building

### MendLoop — AI that fixes real bugs, not toy ones

Finds errors in production code and repairs them. Writing a patch was never the
hard part — knowing whether the patch *worked* is. So it is scored against a
deliberately broken shop app with twenty reproducible bugs, triggered one at a
time, graded on what it actually fixed.

`Python` · *in progress, private*

### [blare](https://github.com/D4RKGEEK/blare) — production errors to Slack in two lines

[![PyPI](https://img.shields.io/pypi/v/blare?color=306998&label=pypi&logo=pypi&logoColor=white)](https://pypi.org/project/blare/)
[![npm](https://img.shields.io/npm/v/%40geekvb%2Fblare?color=cb3837&label=npm&logo=npm&logoColor=white)](https://www.npmjs.com/package/@geekvb/blare)
[![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/D4RKGEEK/blare/blob/main/LICENSE)

Error alerting for Python and Node.js with no server, no database and no
dashboard. Fire the same exception five hundred times and you get **one**
message, not five hundred — which is the whole point, and the thing most
alerting tools get wrong.

Two language implementations held to one written
[specification](https://github.com/D4RKGEEK/blare/blob/main/SPEC.md), with a
conformance suite proving they behave identically. Zero runtime dependencies: a
library that sits in someone else's production path has no business dragging a
tree in with it.

```bash
pip install blare        # or: npm i @geekvb/blare
```

`Python` `TypeScript` · **[live demo](https://d4rkgeek.github.io/blare/)**

### [Tempolight](https://github.com/D4RKGEEK/tempolight) — music-reactive lighting for WLED

[![License: MIT](https://img.shields.io/badge/license-MIT-f5a524.svg)](https://github.com/D4RKGEEK/tempolight/blob/main/LICENSE)
[![Zero dependencies](https://img.shields.io/badge/dependencies-0-brightgreen.svg)](https://github.com/D4RKGEEK/tempolight/blob/main/package.json)
[![Runs on](https://img.shields.io/badge/runs%20on-Windows%20%7C%20macOS%20%7C%20Linux%20%7C%20Raspberry%20Pi-555.svg)](https://github.com/D4RKGEEK/tempolight#install)

A lightweight alternative to LedFx that understands the *song*, not just the
volume — the beat, the bars, the build-ups and the drops. Every LED in the room
is one canvas: strips, rings, frames, poles, panels and matrices.

`Node.js` `TypeScript`

### Candela — the same problem, rebuilt in Rust

A second run at music-reactive lighting, around one idea: **an effect must never
index pixels, only read where they sit in space.** Change which projection it
reads and a chase along a strip becomes a chase across a room — so one effect
works on a strip, a ring, eight poles or a whole club without being rewritten.

Phase-locked beat clock holding tempo to a tenth of a BPM. Drum onsets
classified by spectral shape rather than by which detector fired. OkLab and
OkLch colour, because a red-to-cyan ramp in plain RGB passes straight through
grey. DDP out at 60 fps. **No external crates at all** — the FFT, the JSON
parser, the HTTP server and the colour maths are all hand-written.

`Rust` · *in progress, private*

---

## Also here

**Market data and IPO tooling** — [IPOHut](https://github.com/D4RKGEEK/IPOHut),
[IPOScraper](https://github.com/D4RKGEEK/IPOScraper),
[IPOBackend](https://github.com/D4RKGEEK/IPOBackend),
[market_data](https://github.com/D4RKGEEK/market_data). Scrapers, two backends
and a front end for Indian IPO data — the unglamorous plumbing that turns messy
public filings into something you can actually query.

---

## What I work in

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)
![Rust](https://img.shields.io/badge/Rust-000000?logo=rust&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?logo=kotlin&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?logo=cplusplus&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?logo=gnubash&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?logo=postgresql&logoColor=white)

**Backend and data**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?logo=flask&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-5FA04E?logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?logo=express&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?logo=sqlalchemy&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-FF4438?logo=redis&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?logo=numpy&logoColor=white)

**Front end**

![React](https://img.shields.io/badge/React-61DAFB?logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?logo=nextdotjs&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?logo=vite&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind-06B6D4?logo=tailwindcss&logoColor=white)

**Shipping it**

![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?logo=githubactions&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black)
![Raspberry Pi](https://img.shields.io/badge/Raspberry%20Pi-A22846?logo=raspberrypi&logoColor=white)
![PyPI](https://img.shields.io/badge/PyPI-3775A9?logo=pypi&logoColor=white)
![npm](https://img.shields.io/badge/npm-CB3837?logo=npm&logoColor=white)

**Problems I've actually worked in**

| | |
|---|---|
| **Audio DSP** | FFT, spectral flux, onset detection and classification, tempo and phase tracking |
| **Real-time systems** | 60 fps render loops, UDP streaming, latency budgets, no-allocation hot paths |
| **Observability** | error capture, deduplication, alert fatigue, cross-language conformance |
| **Data extraction** | scraping messy public filings into something queryable |
| **Colour science** | OkLab and OkLch, perceptual gradients, working in linear light |
| **LLM systems** | agents that have to be measured against ground truth, not demoed |

---

## How I work

**I measure the thing I claim.** Not "it feels synced" but the phase error in
beats. Not "onsets are detected" but 5.28 kicks a second measured against the
1.07 that are actually in the track. A test proving only that the output is
finite and in range will pass happily while the effect renders solid black —
that has caught me four separate times, so now I render it and look.

**Zero dependencies, where it matters.** blare, Tempolight and Candela all ship
with none. Candela's FFT, JSON parser, HTTP server and colour maths are
hand-written, because a binary under a megabyte that runs on a Pi Zero is worth
more than the afternoon a crate would have saved.

**Finished means documented.** A spec, a licence, CI, and a demo someone can run
in under a minute. Otherwise it isn't done, it's just working on my machine.

**I'd rather be corrected than agreed with.** Candela's colour work started from
something I believed confidently and had wrong: OkLab does *not* keep a
red-to-blue ramp more saturated than plain RGB. Measuring it is what found the
right answer — OkLch, with hue taken the short way round the circle.

---

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)"
          srcset="https://raw.githubusercontent.com/D4RKGEEK/D4RKGEEK/output/github-snake-dark.svg">
  <source media="(prefers-color-scheme: light)"
          srcset="https://raw.githubusercontent.com/D4RKGEEK/D4RKGEEK/output/github-snake.svg">
  <img alt="A snake eating this year's contribution graph"
       src="https://raw.githubusercontent.com/D4RKGEEK/D4RKGEEK/output/github-snake.svg">
</picture>

<br><br>

[![What I'm listening to](https://spotify-github-profile.kittinanx.com/api/view?uid=31ildgflgg2mo7k6otuxlfr257ua&cover_image=true&theme=default&show_offline=false&background_color=121212&interchange=false&profanity=false&hide_remaster=false)](https://github.com/kittinan/spotify-github-profile)

</div>
