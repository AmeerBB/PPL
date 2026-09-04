# PPL

A single-file workout tracker for the Reddit PPL program. No account, no install, no server — one HTML file that runs in your browser and remembers your lifts.

**[Open it →](https://ameerbb.github.io/PPL.html)**

## What it does

The program runs on session-to-session linear progression, which means the only thing you really need from a tracker is: *what did I lift last time, and what should I load today?* This does that and not much else.

- All six sessions of the cycle — Pull A, Push A, Legs A, Pull B, Push B, Legs B
- Tap in your reps, hit finish, and every load updates itself for next time
- Main lifts add weight each session you hit your reps, and deload 10% after three misses in a row
- Accessories run double progression: top of the rep range on every set, then the weight goes up
- lb / kg toggle, a rest timer, and a running log of past sessions

## Progression rules it applies

| | Lifts | On success | On failure |
|---|---|---|---|
| Linear | Squat, deadlift, bench, row, overhead press | +10 lb squat and deadlift, +5 lb the rest (5 kg / 2.5 kg) | Three misses in a row drops the weight 10% |
| Double | Everything else | Hit the top of the range on all sets, then +5 lb (2.5 kg) | Stay at the same weight and add reps |

Change any weight by hand at any time — typing over a number just overwrites it, and progression carries on from there.

## Using it

Open the link, tap **kg** if you don't work in pounds, and fill in your starting weights. Start the barbell lifts lighter than feels reasonable; the program burns through 5 lb jumps quickly and starting too heavy is the usual reason people stall early.

On a phone, open the page in Safari or Chrome and use **Add to Home Screen**. It gets an icon and runs fullscreen with no browser chrome.

## Where your data goes

Nowhere. Everything is stored in your own browser's local storage on the device you use. There's no backend and nothing is sent anywhere. The flip side: your log lives on one device, and clearing your browser data will erase it. If that worries you, a purpose-built app with cloud sync is the better tool.

## Running your own copy

1. Fork this repo, or download `ppl-log-app.html` and drop it in a new one.
2. Repo **Settings → Pages → Deploy from a branch → main → / (root)**, then save.
3. Wait a minute. Your copy is at `https://YOURUSERNAME.github.io/REPONAME/ppl-log-app.html`.

The whole thing is one file with no dependencies and no build step. Open it in any editor and change the exercise list near the top if you run a variation — each entry is name, sets, rep range, and progression type.

## Credit

The program is [Metallicadpa's linear-progression PPL](https://www.reddit.com/r/Fitness/comments/37ylk5/a_linear_progression_based_ppl_program_for/), posted to r/Fitness in 2015 and still one of the most-run beginner routines around. All programming credit goes there. This is just a logbook for it.

Not affiliated with the author or with r/Fitness. Use it however you like.

## A note

This is a training log, not coaching. It'll happily tell you to add weight when you should be resting, eating more, or fixing your form. Nothing here is medical advice — if something hurts in a way that isn't ordinary training soreness, see someone qualified rather than the spreadsheet.
