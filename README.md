<div align="center">

# Vaibhav

**I build things that run in the real world.**

Error alerting, market data, and a lighting engine that listens to music.
Small tools, finished properly, with claims I can measure.

[blare](https://github.com/D4RKGEEK/blare) ·
[Tempolight](https://github.com/D4RKGEEK/tempolight) ·
[getmendloop@gmail.com](mailto:getmendloop@gmail.com)

</div>

---

## What I'm building

### MendLoop — AI that fixes real bugs, not toy ones

Finds errors in production code and repairs them. The hard part isn't writing a
patch, it's knowing whether the patch worked — so it's measured against a
deliberately broken shop app with twenty reproducible bugs, one at a time.

*In progress, private for now.*

### [blare](https://github.com/D4RKGEEK/blare) — production errors to Slack in two lines

[![PyPI](https://img.shields.io/pypi/v/blare?color=306998&label=pypi&logo=pypi&logoColor=white)](https://pypi.org/project/blare/)
[![npm](https://img.shields.io/npm/v/%40geekvb%2Fblare?color=cb3837&label=npm&logo=npm&logoColor=white)](https://www.npmjs.com/package/@geekvb/blare)
[![CI](https://github.com/D4RKGEEK/blare/actions/workflows/ci.yml/badge.svg)](https://github.com/D4RKGEEK/blare/actions/workflows/ci.yml)
[![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/D4RKGEEK/blare/blob/main/LICENSE)

Error alerting for Python and Node.js with no server, no database and no
dashboard. Fire the same exception five hundred times and you get one message,
not five hundred — which is the whole point, and the thing most alerting
tools get wrong.

```bash
pip install blare        # or: npm i @geekvb/blare
```

**[Live demo](https://d4rkgeek.github.io/blare/)** · [Spec](https://github.com/D4RKGEEK/blare/blob/main/SPEC.md)

### [Tempolight](https://github.com/D4RKGEEK/tempolight) — music-reactive lighting for WLED

[![License: MIT](https://img.shields.io/badge/license-MIT-f5a524.svg)](https://github.com/D4RKGEEK/tempolight/blob/main/LICENSE)
[![Zero dependencies](https://img.shields.io/badge/dependencies-0-brightgreen.svg)](https://github.com/D4RKGEEK/tempolight/blob/main/package.json)
[![Runs on](https://img.shields.io/badge/runs%20on-Windows%20%7C%20macOS%20%7C%20Linux%20%7C%20Raspberry%20Pi-555.svg)](https://github.com/D4RKGEEK/tempolight#install)

A lightweight alternative to LedFx that understands the song rather than just
the volume — the beat, the bars, the build-ups and the drops. Every LED in the
room is one canvas: strips, rings, frames, poles, panels and matrices.

### Candela — the same problem, in Rust

A second run at music-reactive lighting, rebuilt around a single idea: an
effect should never index pixels, only read where they are in space. Change
which projection it reads and a chase along a strip becomes a chase across a
room — so one effect works on a strip, a ring, eight poles or a whole club
without being rewritten.

No external crates. Phase-locked beat clock, classified drum onsets, OkLab
colour, DDP out at 60 fps.

*In progress, private for now.*

---

## Also here

**Market data and IPO tooling** — [IPOHut](https://github.com/D4RKGEEK/IPOHut),
[IPOScraper](https://github.com/D4RKGEEK/IPOScraper),
[market_data](https://github.com/D4RKGEEK/market_data). Scrapers, a backend and
a front end for Indian IPO data.

---

## How I work

**I measure the thing I claim.** Not "it feels synced" but the phase error in
beats. Not "onsets are detected" but 5.28 kicks a second against the 1.07 that
are actually in the track. A test that only proves the output is finite and
in range will pass happily while the effect renders black.

**Zero dependencies, where it matters.** blare and Tempolight both ship with
none. If a tool is meant to sit in someone else's production path, it should
not drag a tree in with it.

**Finished means documented.** A spec, a licence, CI, and a demo you can run
in under a minute — otherwise it isn't done, it's just working on my machine.

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

<sub>Python · TypeScript · Rust · Node.js</sub>

</div>
