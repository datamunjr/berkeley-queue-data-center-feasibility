# 2. Finding and checking possible pairs

[← Back to the summary](./README.md) · [← Previous: Background](./01-background.md)

A "pair" in this study is one data center and one power plant that could, in theory, be built next to each other and connected directly.

## Two ways to find pairs

I looked for pairs from both directions:

1. **Start with a data center, look for a plant.** For 57 data centers that are planned or being built, I took the best nearby solar, wind, or battery project. Those candidates came from [WattConnector](https://wattconnector.munjr.com/), which ranks nearby plants mostly by distance and by how much electricity they could make over a year.
2. **Start with a plant, imagine a data center.** For plants stuck in Berkeley Lab's waiting line, I asked whether a new data center could be built right next to them.

Both kinds of pairs then went through the **same checks**, and the results are reported together.

## The test data center

For pairs that start with a plant, there's no real data center yet, so I used a made-up one to judge every plant the same way:

| Feature | Test data center |
| --- | --- |
| Size | 150 megawatts of computers |
| How hard it runs | 85% of full power on average, around the clock |
| Location | Rural, and willing to build right next to the plant |
| Contract | Willing to buy the plant's power for 15 years |
| Who | A mid-size data center company, not Amazon, Google, Meta, or Microsoft |

Over a year, it uses about **1.12 terawatt-hours** of electricity (150 megawatts × 85% × 8,760 hours in a year).

## Narrowing Berkeley's waiting list

Berkeley Lab publishes the project-level data behind *Queued Up* as a free spreadsheet ([data page](https://emp.lbl.gov/queues)). The 2026 file has about **38,200 rows**: every project that has ever entered a U.S. waiting line, including ones that dropped out long ago and ones already built.

**Step 1: Keep projects still waiting.** That leaves about **9,200** active or paused projects. (The spreadsheet lags reality: some "active" projects turned out to be already built.)

**Step 2: Split by type.**

| Group | About | What I did |
| --- | ---: | --- |
| Solar or wind **with a battery** already planned, or solar and wind together | 2,000 | Kept |
| Solar **only** or wind **only** | 3,800 | Kept, and added a battery on paper |
| **Everything else** | 3,400 | Set aside |

"Everything else" includes about 2,200 stand-alone batteries with no solar or wind next to them, about 650 gas projects, plus hydro, geothermal, nuclear, coal, offshore wind, and others. Stand-alone batteries store power but don't make it, and gas isn't what this study is about.

**Step 3: Group, size, and progress checks.**

- **Group related entries into one plant.** One farm often appears several times, such as one entry for the solar and one for the battery.
- **Keep the right size.** Roughly 120 to 1,200 MW for plants with a battery planned (and at least 50 MW of battery), and roughly 180 to 900 MW for solar-only or wind-only plants. Smaller plants can't power a 150 MW data center. The very largest are usually already linked to the biggest tech companies. When a project left its battery size blank, I estimated it at 90% of the solar or wind size and marked it.
- **Keep plants far along in the process:** a signed or nearly signed grid connection agreement, the final grid engineering study, or construction. Early projects are much more likely to drop out.

That left **482 plants with a battery planned** and **625 solar-only or wind-only plants**. A computer scored each one from 0 to 100 on size, ability to keep the test data center running around the clock, progress, location, and whether a known company is behind it.

**Step 4: Pick plants for a close look.** I picked **48** of those plants: the strongest candidates with a known company behind them, developers worth calling, and a few deliberate test cases, such as plants that looked great on paper but that I suspected were already sold or running.

## All 105 pairs got the same checks

That gave **105 pairs** to check closely: **57** that started with a data center, and **48** that started with a plant.

Each pair was checked for six things that a distance score or spreadsheet can't see:

1. **Is the plant still waiting in line?** A plant that's already running is already selling its power. You can't easily take it back.
2. **Is the power still for sale?** If Amazon or Google already bought the plant, it's off the table.
3. **Can the data center be next to the plant?** A building in a city isn't moving 35 miles into the countryside.
4. **Can it keep the data center running at night?** Making enough electricity over a year isn't the same as making it every hour. Without enough battery, solar can't run a data center at 2 a.m.
5. **Will local rules allow it?** Some states and counties make it very hard to build a data center on farmland.
6. **Is there a real company to work with?** Many projects are owned by small companies with no known parent, or appear only as an ID number.

To apply these checks consistently, I used AI-assisted, role-played review panels: a data center site-selection team, a power seller, and lenders. They are **not** real interviews. See [chapter 6](./06-method-and-limits.md).

## The funnel

```text
Start with a data center               Start with a plant
───────────────────────                ──────────────────
57 planned data centers                ~38,200 entries ever in Berkeley's waiting line
        │                                      │
        │                              ~9,200 still waiting
        │                                      │
        │                              ~5,800 solar or wind (~3,400 other types set aside)
        │                                      │
        │                              1,107 plants after size and progress checks
        │                                      │
57 pairs                               48 picked for a close look
        │                                      │
        └──────────────┬───────────────────────┘
                       ▼
            105 pairs checked the same way
                       │
                       ▼
     2 top picks · 8 worth a meeting · 95 rejected
```

I didn't hand-check 2 terawatts plant by plant. Almost everything was screened out by clear, stated rules, so the close look could focus on a manageable list.

All 105 pairs, with the result and a plain-English reason for each, are in [`data/pairs-reviewed-105.csv`](./data/pairs-reviewed-105.csv).

---

[Next: What held up →](./03-what-held-up.md)
