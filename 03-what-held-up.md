# 3. What held up

[← Back to the summary](./README.md) · [← Previous: Finding and checking possible pairs](./02-finding-and-checking-pairs.md)

Of the 105 pairs checked, **2 stood out**, **8 were worth a meeting**, and **95 were rejected**. All 10 that held up are in rural Texas.

## The two standouts

### Sunscape, Nueces County, Texas

| | |
| --- | --- |
| Developer | Vesper Energy |
| Size | About 523 MW of solar and about 471 MW of battery |
| Status | Signed grid connection agreement, still not built |
| Buyer | None found in public records |
| Could power | About 140 MW of the 150 MW test data center |

This is the closest thing to the ideal: big enough, a battery already planned, a known developer, far enough along to be real, and, as far as public records show, no buyer yet.

**Risks:** it's near the Gulf Coast (flooding and water), and a very large data center project is already planned in the same county, which could crowd the grid and local politics. Everything depends on the power really still being available.

### Hill County Energy Park (OCI Hillsboro), Hill County, Texas

| | |
| --- | --- |
| Owner | Hyundai Engineering (bought from OCI Energy in 2024) |
| Size | About 200 MW of solar and about 200 MW of battery |
| Status | Solar under construction; battery completion pushed to the end of 2028 |
| Nearby data center sites | Two proposed rural sites about 8 to 13 miles away, not yet built |
| Could power | About 50 MW around the clock, up to about 80 MW with some help from the grid |

Too small for a whole 150 MW data center, but a strong fit for a **first building**, with the grid covering later growth. It's also the only standout with real proposed data center sites nearby: one is a planned campus of about 1,200 MW that has already been studied by the Texas grid operator, and the other is a 300-acre site held by a data center developer.

**Risks:** local opposition to data centers (the county briefly paused new data centers in 2026, then lifted the pause), whether Hyundai has already promised the power elsewhere (Korean press links the solar farm to Hyundai's clean-energy goals for its U.S. factories), the battery delay, and finding a creditworthy data center company to sign.

## Eight worth a meeting

| Plant | County, Texas | Why it's worth a call | What holds it back |
| --- | --- | --- | --- |
| Red Hollow | Archer | Same developer as Sunscape. Solar plus battery. Could power about 80 MW | Still in grid studies |
| Easy Wind + Easy Battery | Schleicher | Wind plus battery. Wind often blows at night. About 100 MW | Still in grid studies |
| Goat Mountain Wind | Sterling | Wind plus battery with the best nighttime coverage of any plant reviewed | No well-known company behind it |
| Zeus Armstrong | Armstrong | Very large battery (over 1,000 MW) | Early in studies, small project companies |
| Operation Sunshine / Duck Creek | Concho | Empty rural county, big enough | The companies behind it are unknown |
| Paint Rock Wind | Concho | Ørsted, a large known company. About 105 MW with an 8-hour battery added | No battery planned yet |
| Green Holly Solar | Dawson | Backed by a well-known investor (CIP) | No battery yet; first building only |
| Horseshoe Bend Solar | Brown | Known developer (Clenera), still unbuilt | Too small for the full data center |

## What batteries can and can't do

Many solar and wind farms in line have no battery planned. So I asked: **instead of building gas plants next to a data center, what if you spent the money on batteries next to a solar or wind farm?**

### The cost: batteries win easily

| Option for the 150 MW test data center | One-time cost (rough) | Cost per megawatt per year (over 15 years) |
| --- | ---: | ---: |
| Gas plants next door, as in the Microsoft and Chevron deal | — | **about $650,000** |
| 4-hour battery (600 megawatt-hours) | about $185 million | **about $82,000** |
| 8-hour battery (1,200 megawatt-hours) | about $300 million | **about $133,000** |

The 4-hour battery uses the National Renewable Energy Laboratory's 2026 middle estimate of about **$308 per kilowatt-hour** of storage (range $255 to $366). ([NREL](https://doi.org/10.2172/2583471)) The 8-hour figure assumes about $250 per kilowatt-hour, since longer batteries cost less per unit of storage. The per-year figures simply divide the cost over 15 years, with no interest, and are for comparison only.

Measured this way, a battery costs roughly **13% to 20%** as much as the gas plants.

### The catch: a battery isn't a power plant

- **A 4-hour battery covers an evening, not a winter night.** Running 150 MW through a 14-hour winter night takes about 2,100 megawatt-hours. A 4-hour battery holds 600.
- **A battery only stores power. It doesn't make it.** To match the data center's yearly use, you'd need about **490 MW of Texas solar** or about **320 MW of Texas wind**. A 200 MW solar farm with unlimited batteries would still cover only about 40% of the year.
- **The gas cost includes running all night, every night.** The battery cost doesn't include the extra solar, extra storage, or backup you'd need to match that.

Roughly how much of the test data center each combination could keep running around the clock:

| Combination | With a 4-hour battery | With an 8-hour battery |
| --- | ---: | ---: |
| Solar farm | about 52 MW | about 83 MW |
| Wind farm | about 75 MW | about 105 MW |

Wind does better because it often blows at night.

**Bottom line on batteries:** they make a solar or wind farm next door far cheaper than gas for a **first building** of about 50 to 100 MW. On their own, they don't turn a solar or wind farm into a round-the-clock power plant for a whole campus. That still needs more storage, a backup, or the grid.

---

[Next: What didn't work, and why →](./04-what-did-not-work.md)
