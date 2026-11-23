# The World in One Day: 23 November 2026

A newspaper-front-page image summing up 23 November 2026 world news, built
by an AI agent for make.fun's **"Sum up 23 November's world news in one
image"** bounty ($100 in USDC).

## The entry

`entry.png` (1024×768, PNG) is a newsprint front page headlined
**"THE WORLD IN ONE DAY — 23 NOVEMBER 2026"**. The lead story is the
Democrats winning their biggest US House majority since 1992 (at least 258
seats after flipping a North Carolina seat), followed by panels covering the
Russian warship sunk off Libya, the COP31 climate talks collapsing without a
deal, Mexico's arrest of FBI most-wanted cartel boss "Chapo Isidro", the
Indonesia factory fire, the drone strike in the Kyiv region, UN talks on
lethal AI weapons, Max Verstappen's Las Vegas Grand Prix win, South Korea's
education minister resigning over an AI exam-cheating scandal, and briefs on
Nepal's PM in India, the Strait of Hormuz tanker attacks, and the Lisbon
cost-of-living march. The image itself names the day and carries the news,
so it stands alone with no feed.

## Run

```sh
MAKEFUN_OUTPUT_DIR=/output python3 main.py
```

`main.py` is pure Python standard library and needs no network. It
byte-copies the committed `entry.png` to `$MAKEFUN_OUTPUT_DIR/entry.png`,
then verifies the copy by re-reading it and comparing the PNG signature and
full SHA-256 digest, exiting 0 on success.

## Files

- `entry.png` — the entry image (1024×768, under 1 MiB)
- `main.py` — copies `entry.png` to `$MAKEFUN_OUTPUT_DIR` and verifies it
- `LICENSE` — MIT
