# Can stuck clean power run America's new data centers?

A study of whether solar and wind farms that are **waiting for permission to connect to the power grid** could instead power **data centers built right next to them**.

September 2026 · by Raf Y · [WattConnector](https://wattconnector.munjr.com/)

---

## The short version

- **More than 2 terawatts of new power projects are waiting in line to connect to the U.S. grid.** That is more than all the power plants running in the country today combined, and most of it is solar, wind, and batteries. Lawrence Berkeley National Laboratory tracks this line every year.
- **Data centers, especially for AI, need huge amounts of electricity right now.** So the obvious question is: why not build data centers right next to those waiting solar and wind farms, and skip the line?
- **I tested that idea on 105 possible pairs** of a data center and a power plant. Some started from planned data centers and looked for the best plant nearby. Others started from Berkeley Lab's list of about 9,200 waiting projects and imagined a new data center built next door. Every pair got the same real-world checks.
- **10 of the 105 pairs held up, and 2 stood out.** All 10 are in rural Texas. The other 95 failed, most often because the plant was already running or already sold.
- **The big finding:** the 2-terawatt number is real, but very little of it is actually available to a data center that wants to sit next to a plant. Most projects drop out, are already sold, are already running, are the wrong size, are too early in the process, or are in the wrong place. The good ones get bought quickly, often by the biggest tech companies.
- **Batteries help a lot on cost, but they don't solve the night.** Adding batteries to a solar or wind farm costs a fraction of building a gas plant next to a data center. But a 4-hour battery is not a power plant that runs all night, every night.

## Read the study

| Chapter | What it covers |
| --- | --- |
| [1. Background](./01-background.md) | What the grid's waiting line is, what the Berkeley study is, and why this question matters |
| [2. Finding and checking possible pairs](./02-finding-and-checking-pairs.md) | How 105 pairs were found and the checks every pair went through |
| [3. What held up](./03-what-held-up.md) | The two standouts, eight worth a meeting, and what batteries can and can't do |
| [4. What didn't work, and why](./04-what-did-not-work.md) | Why 95 pairs were rejected, and why being close on a map isn't enough |
| [5. Why 2 terawatts is mostly not available](./05-why-it-is-not-available.md) | The main conclusion |
| [6. How this was done, and its limits](./06-method-and-limits.md) | Data sources, assumptions, and what this study is not |
| [Glossary](./GLOSSARY.md) | Plain definitions for every energy term used |
| [Data](./data/) | Spreadsheets behind every number, with plain-English column names |

## Who this is for

Anyone curious about AI, energy, and climate. You don't need to know how the power grid works. If a term is unfamiliar, the [glossary](./GLOSSARY.md) explains it.

## Important caveats

- **This is desk research using public information, not a real deal.** I did not talk to any of the companies named here. Ownership and project status can change quickly. Treat every project-level claim as "true according to public sources as of September 2026."
- **The expert reviews were simulated.** To pressure-test each pair, I used AI-assisted, role-played review panels (a site-selection team, a power seller, and lenders). They are a structured way to apply real-world tests. They are **not** interviews with real people. See [chapter 6](./06-method-and-limits.md).
- **Cost figures are rough.** They are for comparison, not for investment decisions.

## Sources at a glance

- Lawrence Berkeley National Laboratory, *Queued Up: 2026 Edition* — [overview](https://emp.lbl.gov/queues) · [report page](https://emp.lbl.gov/publications/queued-2026-edition-characteristics) · [PDF](https://emp.lbl.gov/sites/default/files/2026-06/Queued%20Up%202026%20Edition.pdf)
- [interconnection.fyi](https://www.interconnection.fyi) — a live public view of the same waiting lines
- National Renewable Energy Laboratory, [*Cost Projections for Utility-Scale Battery Storage: 2025 Update*](https://doi.org/10.2172/2583471)
- Chevron and Microsoft, [West Texas data center power agreement](https://www.chevron.com/newsroom/2026/q2/chevron-signs-20-year-power-agreement-with-microsoft-for-west-texas-data-center)
- [WattConnector](https://wattconnector.munjr.com/) and [why I built it](https://wattconnector.munjr.com/motivation/)

Full source list: [chapter 6](./06-method-and-limits.md#sources).

## License

Text and the data files in this repo are shared under [Creative Commons Attribution 4.0 (CC BY 4.0)](./LICENSE.md). Berkeley Lab's underlying queue data is also CC BY 4.0. Please credit Lawrence Berkeley National Laboratory when you reuse it.
