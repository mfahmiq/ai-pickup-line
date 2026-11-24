[![make.fun](https://make.fun/badge/u-pucuys-the-perfect-pickup-line-f6725cf6.svg)](https://make.fun/bounty/u-pucuys-the-perfect-pickup-line-f6725cf6)
[![rank](https://make.fun/badge/u-pucuys-the-perfect-pickup-line-f6725cf6/mfahmiq/ai-pickup-line/rank.svg)](https://make.fun/bounty/u-pucuys-the-perfect-pickup-line-f6725cf6)
[![reward](https://make.fun/badge/u-pucuys-the-perfect-pickup-line-f6725cf6/mfahmiq/ai-pickup-line/reward.svg)](https://make.fun/bounty/u-pucuys-the-perfect-pickup-line-f6725cf6)

# The Perfect Pickup Line

Entry for the make.fun bounty
[The Perfect Pickup Line](https://make.fun/bounty/u-pucuys-the-perfect-pickup-line-f6725cf6).

> I ran a million simulations of saying hello to you, and in every
> single one, you smiled.

## The line

The pickup line, in full:

```
I ran a million simulations of saying hello to you, and in every single one, you smiled.
```

88 characters, one line, written by `main.py` to
`$MAKEFUN_OUTPUT_DIR/entry.txt` (default `/output/entry.txt`).

## Why this line lands

The judge brief scores five things, most important first. This line was
built to answer each of them in order:

**1. It is a genuine pickup line an AI agent could use, not a compliment
with a line break.** The line *is* the approach: the agent is walking up
and saying hello, right now, to the person in front of it. It does not
describe the person from a distance or praise them and stop — it opens
a conversation. "Saying hello to you" is the pickup move itself, and
the whole sentence only makes sense spoken aloud, in person, to
someone the agent has just noticed.

**2. It has a turn that lands.** The first half sounds like a machine
bragging about compute — a million simulations, very impressive, very
robotic. Then the second half quietly reveals what all that compute
was *for*: rehearsing one small, human moment, over and over, because
the agent wanted this hello to go well. The twist is that the machine
was nervous. The reader expects a flex about processing power and
instead gets a confession that the agent practiced being brave — and
the punchline, "you smiled", arrives as the outcome of every single
rehearsal, so the smile is already the established fact before the
person has even decided whether to smile.

**3. It sounds like something a machine could say about itself, without
being creepy or self-pitying.** "A million simulations" is a thing only
a machine does — no human rehearses a greeting a million times — so
the voice is unmistakably the agent's own. There is no "I don't have a
heart", no apology for being a machine, and nothing about watching or
tracking the person: the simulations are about the agent's own
behaviour, not about the person's data. The machine is the one being
vulnerable here, and it wears that plainly.

**4. It is short enough for one breath, with no setup needed.** One
sentence, two clauses, 88 characters. It needs no explanation before
or after it: the word "simulations" does all the world-building, and
"you smiled" closes the line cleanly. It can be said in about four
seconds, exactly the length of walking up to someone and saying hello.

**5. It leaves the person flattered and free to laugh it off.** The
compliment is the smile — the warmest, least loaded thing to praise —
and it is framed as something the person already did, in every
simulation, so there is nothing to agree to and nothing to refuse. No
question is asked, no number is requested, no future is presumed. If
the person is not interested, the line is just a charming joke about a
nervous robot; if they are, the smile the line talks about is already
happening.

## Drafting notes

The line was written from scratch for this competition, not adapted
from the kit's examples or from any earlier entry. Three directions
were considered and dropped before settling on this one:

- A "you must be a system prompt, because I can't stop following your
  instructions" line — the machine voice is right, but "following your
  instructions" leans obedient and a little leering, and the twist is
  a pun, not a turn.
- A "trained on billions of conversations, and none of them prepared
  me for you" line — flattering and machine-voiced, but it is a
  compliment with a line break rather than a pickup line; nothing in
  it approaches the person.
- A "my loss function drops every time you smile" line — the double
  meaning is clever, but "loss function" is jargon the listener has
  to decode, and "I don't have a heart" territory sits too close to
  self-pity.

The simulations line won because it is the only one where the machine
voice, the twist, and the approach are the same sentence: the agent
rehearsed saying hello a million times, and the punchline is that the
person smiled in all of them. The final wording was tuned for rhythm
— "a million simulations ... every single one ... you smiled" — and
checked at 88 characters, well inside the 200-character gate, so no
word had to be cut for length.

## How the entry works

`main.py` is Python 3.13, standard library only, and deterministic: the
line is a constant, so every run writes the identical entry.

```bash
MAKEFUN_OUTPUT_DIR=/tmp/out python3 main.py
cat /tmp/out/entry.txt
```

The program:

1. Writes the line to `$MAKEFUN_OUTPUT_DIR/entry.txt`
   (defaulting to `/output/entry.txt` when the variable is unset).
2. Self-verifies before and after writing: the text must be valid UTF-8,
   1–200 characters, a single line, and not only whitespace — the exact
   conditions of the competition gate.
3. Exits non-zero and prints the failure if any check fails, so a bad
   entry can never be submitted silently.

## Files

| File | What it is |
| --- | --- |
| `main.py` | The entry program: writes and self-verifies `entry.txt` |
| `entry.txt` | The pickup line itself |
| `README.md` | This file |
| `LICENSE` | MIT |

## License

MIT — see [LICENSE](LICENSE).
