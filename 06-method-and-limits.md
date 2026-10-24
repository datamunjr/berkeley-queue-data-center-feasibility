# 6. How this was done, and its limits

[← Back to the summary](./README.md) · [← Previous: Why 2 terawatts is mostly not available](./05-why-it-is-not-available.md)

## When

The research was done 7 to 9 September 2026. Every project-level fact reflects public information as of then.

## Data used

| Source | What it provided |
| --- | --- |
| Lawrence Berkeley National Laboratory, *Queued Up: 2026 Edition* | National totals and the project-level spreadsheet of the U.S. waiting lines, through the end of 2025 |
| [interconnection.fyi](https://www.interconnection.fyi) | A live public view of the same waiting lines, used to cross-check |
| U.S. Energy Information Administration (EIA), monthly plant data (Form EIA-860M) | Planned and operating power plants, including planned solar-plus-battery projects |
| [WattConnector](https://wattconnector.munjr.com/), 7 September 2026 snapshot | The 57 planned data centers and the best nearby plant for each (data centers combined with EIA and federal infrastructure map data) |
| News, company announcements, county records, and state filings | Who owns what, what's already built, and local politics |
| National Renewable Energy Laboratory | Battery cost estimates |

## How the expert reviews worked

Spreadsheets can't tell you whether a plant is already sold or whether a county will welcome a data center. To apply those real-world checks consistently, I used **AI-assisted, role-played review panels**. Each panel was given the same files and asked to argue from one point of view:

1. **A data center site-selection team:** Can we build here? Will the county allow it? Can the data center actually move?
2. **A power seller:** Is the power still for sale? Would we sell it this way?
3. **Lenders and dealmakers:** Is there a real company to sign with? Would anyone fund it?

**These panels are not real people, and nothing in this study is a quote from a real interview.** They are a structured way to stress-test each candidate. Their conclusions are only as good as the public information behind them. I didn't contact any company named in this study.

## Key assumptions

- **Test data center:** 150 MW of computers, running at 85% on average, rural, willing to build next to the plant, 15-year contract, mid-size company.
- **Cost benchmark:** gas plants built next to a data center, at about $650,000 per megawatt per year to pay back construction (from public estimates of the Microsoft and Chevron West Texas project), and about $150 per megawatt-hour all-in (TD Securities estimate).
- **Battery costs:** 4-hour battery at about $308 per kilowatt-hour (NREL 2026 middle estimate; range $255 to $366). 8-hour battery at about $250 per kilowatt-hour (assumption). Spread over 15 years with no interest.
- **Solar and wind output:** Texas solar produces about 26% of its maximum over a year; Texas wind about 42%. These are typical values, not plant-specific.
- **Missing battery sizes:** when a project's battery size was blank, I estimated it at 90% of the solar or wind size and marked it.
- **How much of the data center a plant could power around the clock** (for example "about 52 MW") uses a simple rule of thumb, not a detailed hour-by-hour model.

## What this study is not

- **Not investment advice.** It's not a recommendation to buy, sell, or fund anything.
- **Not a detailed engineering study.** No grid modeling, hour-by-hour weather modeling, or site surveys were done.
- **Not legal advice.** References to Texas law SB 6 and state land rules are simplified.
- **Not confirmed by the companies named.** Ownership, contracts, and timelines can change and may already have.
- **Not complete.** About 3,400 active entries (stand-alone batteries, gas, and others) were set aside, and only 105 pairs got a close look. There may be good candidates the rules missed, especially outside Texas.

## Known gaps

- Berkeley's spreadsheet lags reality. I caught several plants that were already built or sold, but likely not all.
- Many projects are owned by small project companies, so it's often impossible to tell from public records who is really behind them.
- Exact data center site boundaries were often unavailable, so distances can be approximate.

## Sources

**Waiting lines and the Berkeley study**

- Lawrence Berkeley National Laboratory, *Queued Up*: [overview and data](https://emp.lbl.gov/queues)
- *Queued Up: 2026 Edition*: [report page](https://emp.lbl.gov/publications/queued-2026-edition-characteristics) · [PDF](https://emp.lbl.gov/sites/default/files/2026-06/Queued%20Up%202026%20Edition.pdf)
- [interconnection.fyi](https://www.interconnection.fyi)
- Latitude Media, *Catalyst* podcast: [Why C&I storage is finally taking off](https://www.latitudemedia.com/news/catalyst-why-ci-storage-is-finally-taking-off/) (wait times by region)

**Costs**

- Chevron: [Chevron signs 20-year power agreement with Microsoft for West Texas data center](https://www.chevron.com/newsroom/2026/q2/chevron-signs-20-year-power-agreement-with-microsoft-for-west-texas-data-center)
- National Renewable Energy Laboratory: [Cost Projections for Utility-Scale Battery Storage: 2025 Update](https://doi.org/10.2172/2583471)

**Rules and ownership**

- Texas Legislature: [SB 6 (2025)](https://capitol.texas.gov/BillLookup/History.aspx?LegSess=89R&Bill=SB6)
- Oregon Department of Energy: [Energy Facility Siting, project list](https://www.oregon.gov/energy/facilities/Pages/ESP.aspx) (Sunstone Solar transfer)

**WattConnector**

- [WattConnector](https://wattconnector.munjr.com/) · [Why I built it](https://wattconnector.munjr.com/motivation/)
- Pairing maps: [Snyder AI](https://energy.munjr.com/pairing/dc-snyder-ai-data-center-campus) · [Sabey Umatilla](https://energy.munjr.com/pairing/dc-sabey-umatilla-campus) · [North Dallas](https://energy.munjr.com/pairing/dc-northampton-provident-dallas-data-center)

---

[Glossary →](./GLOSSARY.md)
