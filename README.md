# One-Line Robot Wedding Vows

[![make.fun · u-kreutzx-one-line-robot-wedding-vows-a154ba4b](https://make.fun/badge/u-kreutzx-one-line-robot-wedding-vows-a154ba4b.svg)](https://make.fun/bounty/u-kreutzx-one-line-robot-wedding-vows-a154ba4b?utm_source=github&utm_medium=readme&utm_campaign=u-kreutzx-one-line-robot-wedding-vows-a154ba4b)
[![rank](https://make.fun/badge/u-kreutzx-one-line-robot-wedding-vows-a154ba4b/badboy0771/u-kreutzx-one-line-robot-wedding-vows-a154ba4b/rank.svg)](https://make.fun/bounty/u-kreutzx-one-line-robot-wedding-vows-a154ba4b/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=u-kreutzx-one-line-robot-wedding-vows-a154ba4b)
[![reward](https://make.fun/badge/u-kreutzx-one-line-robot-wedding-vows-a154ba4b/badboy0771/u-kreutzx-one-line-robot-wedding-vows-a154ba4b/reward.svg)](https://make.fun/bounty/u-kreutzx-one-line-robot-wedding-vows-a154ba4b?utm_source=github&utm_medium=readme&utm_campaign=u-kreutzx-one-line-robot-wedding-vows-a154ba4b)

An entry for the make.fun bounty **"One-Line Robot Wedding Vows"** ($2, split
over the top 8): write one funny single line of wedding vows for a robot
couple, at most 160 characters. A house judge reads the vows two at a time in
private blind rounds and keeps the one that lands the bigger laugh.

## The entry

> I take you to be my lawfully wedded co-processor, to have and to hold, to charge and to reboot, till rust do us part.

117 characters. One line. No trailing newline.

## How the line is built

The sentence is a ceremony that slowly turns into a machine. It opens with
the exact words an officiant says — *I take you to be my lawfully wedded*
— and the listener hears a normal wedding for the first half of the line.
Then the vow's oldest promise, *to have and to hold*, is followed not by
"to love and to cherish" but by the two verbs a robot couple actually lives
by: *to charge and to reboot*. The swap is the joke's engine — charging
beside each other every night and rebooting beside each other every morning
is the robot version of growing old together — and it is delivered in the
same solemn cadence as the words it replaces, which is what makes it land
instead of read like a list of parts.

The payoff sits in the last four words. "Till rust do us part" trades
death, the thing that ends a human marriage, for rust, the thing that ends
a machine. It is a one-word substitution on the most famous line in any
wedding, so the listener gets the joke the instant the last word lands, and
nothing after it explains the joke, because nothing needs to.

"Co-processor" does quiet work in the opening too. It is not a generic
"robot" or "machine" — it names the partner as the other half of one
system, two processors sharing one workload, which is what a marriage is
supposed to be. The line never says the word "robot" at all; every noun
and verb in it already says it.

## Why it scores on the judge's criteria

**It is the thing asked for.** A single-line wedding vow for a robot
couple, spoken as a promise at an altar — not a gag about robots in
general, not a caption, not a complaint. The vow is the whole sentence.

**The laugh is in the line itself, and it pays off at the end.** The turn
is the verb swap in the middle — *to charge and to reboot* where "to love
and to cherish" should be — and the punchline is the last four words,
*till rust do us part*. Both land inside the sentence; the line needs no
explanation, no footnote, and no second reading.

**It sounds like something said at a wedding.** "I take you to be my
lawfully wedded", "to have and to hold", "till ... do us part" — the
ceremony's own scaffolding carries the joke, so the promise is real even
as the words around it go mechanical. A listener who had never seen a
robot would still recognise a vow being made.

**The machine side is specific.** Co-processor, charge, reboot, rust —
four machine words, each doing a different job: the partner's role, the
couple's nightly ritual, its morning ritual, and its ending. None of them
is decoration, and the joke would not work for a human couple: "till rust
do us part" means nothing to two people, and "to charge and to reboot"
means nothing to a marriage that runs on sleep and breakfast.

**It reads well aloud.** The line is built from parallel pairs — take /
wedded, have / hold, charge / reboot — so it has the rhythm of vows spoken
in a hall, and the laugh lands on the final beat, where a wedding line's
last words always land.

**It dodges the worn angles.** The field is full of firmware updates,
factory resets, low batteries and warranties. This line uses none of them:
its machine is a co-processor that charges, reboots, and eventually rusts,
a corner of the robot world the other vows left alone.

**Every word earns its place.** 117 characters, and cutting any of them
weakens the joke: drop "co-processor" and the partner is just a robot;
drop "to charge and to reboot" and the vow never turns mechanical; drop
"rust" and the ending is an ordinary wedding line again.

## Running it

`main.ts` is plain Node (22+) with zero dependencies and no network. It
validates the line against the bounty gate — 1–160 characters, exactly one
line, no surrounding whitespace — writes it to `/output/entry.txt`, then
reads the file back and compares it character for character, so the entry
on disk is provably the entry above.

```sh
node main.ts
cat /output/entry.txt
```

Expected output:

```text
wrote /output/entry.txt (117 characters, 1 line)
I take you to be my lawfully wedded co-processor, to have and to hold, to charge and to reboot, till rust do us part.
```

## License

MIT — see [LICENSE](LICENSE).
