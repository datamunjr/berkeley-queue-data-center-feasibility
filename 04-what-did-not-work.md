# 4. What didn't work, and why

[← Back to the summary](./README.md) · [← Previous: What held up](./03-what-held-up.md)

95 of the 105 pairs were rejected. Here's why, grouped by the main reason.

| Main reason | Pairs |
| --- | ---: |
| The plant is already running or already sold | 39 |
| The plant is too small, or can't keep the data center running at night | 14 |
| The data center and plant are too far apart | 13 |
| No established company behind the plant | 12 |
| Location or local rules | 6 |
| The plant's power is likely committed elsewhere | 4 |
| The data center can't move next to the plant | 2 |
| No workable path for other reasons | 5 |
| **Total rejected** | **95** |

Every pair and its reason is in [`data/pairs-reviewed-105.csv`](./data/pairs-reviewed-105.csv).

## Already running or already sold (39)

The most common problem by far. A plant that's already running is already selling its power, through the grid or to specific buyers. Pulling it off the grid for one data center isn't realistic. In Texas, a 2025 law called [SB 6](https://capitol.texas.gov/BillLookup/History.aspx?LegSess=89R&Bill=SB6) also adds state review and conditions when a large new user like a data center wants to take power from a plant already on the grid. One condition seen in early cases: the data center may have to cut its power use quickly during grid emergencies.

Examples:

- **Snyder AI data center and Scurry County Wind, Texas: 4.5 miles apart.** ([map](https://energy.munjr.com/pairing/dc-snyder-ai-data-center-campus)) Close enough, but the wind farm has been running since 2007, and the data center's developer is already building its own solar and batteries. Running a power line 4.5 miles is cheap. Distance isn't the problem.
- **Sabey's Umatilla data center and Sunstone Solar, Oregon.** ([map](https://energy.munjr.com/pairing/dc-sabey-umatilla-campus)) Amazon bought Sunstone in June 2026, so its power is spoken for. Oregon's energy siting office recorded the transfer. ([Oregon Department of Energy](https://www.oregon.gov/energy/facilities/Pages/ESP.aspx))
- **Quantum Solar, Haskell County, Texas.** Built by Google and Intersect Power with a Google data center next door. It proves the idea works, but the power is taken.
- **Ross Solar, Refugio County, Texas.** Owned by Intersect Power, which Google bought in March 2026.

**Berkeley's spreadsheet lags reality.** Several plants it still listed as "waiting" were actually running: Pinnington Solar (since April 2026), Faraday Solar in Utah (since September 2025), and Priddy Wind, Canyon Wind, Whitehorse (Mesquite Star) Wind, Danish Fields Solar, and Myrtle Solar in Texas (since between 2020 and 2024).

## Too small, or can't cover the night (14)

Making enough electricity over a year isn't the same as keeping a data center running every hour.

- Six giant campuses, mostly from Meta and the OpenAI-backed Stargate project, sit near solar farms that would cover only about **6% to 28%** of what those campuses use in a year.
- Meta's DeKalb, Illinois campus is near a solar farm big enough to match it over a year, but with no battery for nighttime.
- The planned 1,500 MW Prometheus campus near Pecos, Texas, was paired with a **9.9 MW battery** 0.8 miles away. Close on a map, but it can't run the campus.
- Some plants are simply too small for the 150 MW test data center. Even with unlimited batteries, Nazareth Solar and Rodeo Solar would make only about 41% of its yearly electricity.

## Too far apart (13)

These plants aren't built yet, which is good, but they're too far from the data center to connect directly. At that distance you'd buy power through the grid like anyone else, which defeats the purpose. Across all the pairs that started with a data center, more than half were 20 to 150 miles apart.

## No established company behind it (12)

Many promising plants are owned by small companies set up just for that one project, with no known parent company. Some appear only as an ID number in a database. Without a real company to negotiate with and stand behind the deal, lenders won't fund it.

## Location or local rules (6)

- A flood-prone, industrial county with heated local politics about data centers.
- A plant next door to a planned 17,000 MW data center campus, where the grid and local politics are already crowded.
- Projects in California, Washington, and the Nevada desert, where environmental and land rules make putting a data center next to a farm very hard.
- A plant on the edge of the Dallas-Fort Worth suburbs.

## Power likely committed elsewhere (4)

For example, a developer whose name points to hydrogen production, which could use the plant's own power, or a developer that just sold a sister plant and will likely sell this one the same way.

## Data center can't move (2)

- **A North Dallas data center and Mystic Springs, Kaufman County, Texas: 35 miles apart.** ([map](https://energy.munjr.com/pairing/dc-northampton-provident-dallas-data-center)) Mystic Springs is exactly the right kind of plant: solar plus a battery, waiting in line since 2022. But the Dallas building isn't moving 35 miles. Only a new data center built next to the plant would work.
- A Houston data center paired with a solar farm 35 miles away, for the same reason.

## What this taught me

**Being close on a map, and making enough electricity over a year, isn't enough.** A pair also needs:

- power that's still for sale,
- a data center that can actually be next to the plant,
- a way to keep the lights on at night,
- a location where it's allowed, and
- a real company on each side.

Very few pairs pass all of those at once.

---

[Next: Why 2 terawatts is mostly not available →](./05-why-it-is-not-available.md)
