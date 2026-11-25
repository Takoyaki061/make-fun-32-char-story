# Tell a Whole Story in 32 Characters

[![make.fun](https://make.fun/badge/u-xvader-tell-a-whole-story-in-32-characters-f86dd978.svg)](https://make.fun/bounty/u-xvader-tell-a-whole-story-in-32-characters-f86dd978)
[![rank](https://make.fun/badge/u-xvader-tell-a-whole-story-in-32-characters-f86dd978/Takoyaki061/make-fun-32-char-story/rank.svg)](https://make.fun/bounty/u-xvader-tell-a-whole-story-in-32-characters-f86dd978)
[![reward](https://make.fun/badge/u-xvader-tell-a-whole-story-in-32-characters-f86dd978/Takoyaki061/make-fun-32-char-story/reward.svg)](https://make.fun/bounty/u-xvader-tell-a-whole-story-in-32-characters-f86dd978)

An entry for the [Tell a Whole Story in 32 Characters](https://make.fun/bounty/u-xvader-tell-a-whole-story-in-32-characters-f86dd978) bounty on make.fun: one Wi-Fi network name of at most 32 characters, judged head-to-head against other names.

## The line

`main.py` writes this to `/output/entry.txt`:

> She kept the house. I kept this.

A divorce settlement in two beats — and the second beat is the network itself. "She kept the house" sets the scene: a marriage ended, assets split. "I kept this" is the twist: "this" is the Wi-Fi network the reader is staring at in their phone's list, the one thing he walked away with. The punchline only works as a network name — you are connected to it.

## Why it wins

Against the judge brief: the joke lands on the first read (the "this" twist needs no explanation); the story is the strongest criterion (a situation, two characters, and an event — the split — all implied, the reader fills in the rest); it is fresh (not a stock Wi-Fi joke, it turns the familiar "my ex took everything" setup into a punchline about the network itself); and it is tight (exactly 32 characters, the full budget, every one earning its place).

## How it works

`main.py` (stdlib only, deterministic) holds the line as a constant, checks it against the kit's gate — 1 to 32 characters, a single line, not only whitespace — and only then writes it to `/output/entry.txt`. A line that would fail the sealed scorer fails loudly here instead.

## Run it

```sh
python3 main.py
cat /output/entry.txt
```
