# Data

[← Back to the summary](../README.md)

The spreadsheets behind the study, as CSV files that open in Excel, Google Sheets, or Numbers. Sizes are in megawatts (MW). See the [glossary](../GLOSSARY.md) for terms.

| File | Rows | What it is |
| --- | ---: | --- |
| [`pairs-reviewed-105.csv`](./pairs-reviewed-105.csv) | 105 | Every data center and power plant pair that got a close look, with the result and a plain-English reason |
| [`plants-scored-with-battery-482.csv`](./plants-scored-with-battery-482.csv) | 482 | Plants from Berkeley's waiting list with solar or wind and a battery planned that passed the size and progress checks |
| [`plants-scored-solar-wind-only-625.csv`](./plants-scored-solar-wind-only-625.csv) | 625 | Solar-only or wind-only plants from Berkeley's waiting list that passed the size and progress checks, with a battery added on paper |

## `pairs-reviewed-105.csv`

Sorted with the top picks first, then the pairs worth a meeting, then the rejected pairs grouped by reason.

| Column | Meaning |
| --- | --- |
| `result` | **Top pick**, **Worth a meeting**, or **Rejected** |
| `reason_category` | For rejected pairs, the main reason, in one of eight groups (see [chapter 4](../04-what-did-not-work.md)) |
| `reason` | A plain-English explanation |
| `data_center` | The data center's name. For pairs that started with a plant, this is the made-up 150 MW test data center built next door |
| `data_center_company`, `data_center_location`, `data_center_size_mw`, `data_center_status` | Who's building it, where, how big, and how far along |
| `power_plant`, `power_plant_owner`, `power_plant_location` | The plant's name, the company listed as owner (often a company set up just for that project), and county and state |
| `power_plant_type` | Solar, wind, battery, or a combination |
| `solar_mw`, `wind_mw`, `battery_mw` | Planned sizes. "(estimated)" means Berkeley's data left the battery size blank and it was estimated at 90% of the solar or wind size |
| `power_plant_status` | Already running, under construction, or how far along it is in the waiting line |
| `miles_apart` | Straight-line distance between the two, or "next door" for the test data center |
| `share_of_data_center_yearly_need` | How much electricity the plant makes in a year compared with what the data center uses. Over 100% doesn't mean it covers every hour, for example at night. Blank where not calculated |
| `map_link` | The pair on the WattConnector map, where available |

## The two scored plant files (482 and 625 plants)

These are computer-scored lists of plants from Berkeley's waiting list, **before** the close look. A high score here doesn't mean a plant is a good deal: the close look rejected several high scorers because they were already sold, already running, or had no real company behind them. Plants marked `reviewed_closely = yes` are among the pairs in `pairs-reviewed-105.csv`.

For example, Briggs Solar and Solace Solar in Haskell County, Texas, score well but weren't reviewed. Their owner names ("IP Quantum") suggest they belong to the same Intersect Power family as Google's Quantum project, so treat them as likely spoken for.

| Column | Meaning |
| --- | --- |
| `computer_rank` | Rank by score within the file |
| `berkeley_queue_ids` | The project's ID number(s) in Berkeley's dataset, so you can look it up |
| `battery_size_estimated` | `yes` if the battery size was blank in Berkeley's data and estimated at 90% of the solar or wind size |
| `est_data_center_mw_it_could_power` | Rough estimate of how many MW of the 150 MW test data center the plant could keep running around the clock |
| `type`, `plant_mw` | Solar or wind, and size (625 file only) |
| `share_of_test_data_center_yearly_need` | How much of the test data center's yearly electricity the plant would make (625 file only) |
| `data_center_mw_with_4h_battery`, `data_center_mw_with_8h_battery` | Rough estimate of how many MW of the test data center it could keep running around the clock with a 4-hour or 8-hour battery added (625 file only) |
| `score_0_to_100` | Screening score. For plants that got a close look, this is the score after that review |
| `reviewed_closely` | Whether this plant got a close look |

## Credit and license

Plant-level waiting-line data comes from Lawrence Berkeley National Laboratory's *Queued Up* dataset ([emp.lbl.gov/queues](https://emp.lbl.gov/queues)), shared under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Please credit Berkeley Lab when you reuse it. Scores, results, and reasons are this study's own and are shared under the same license. Ownership and status reflect public information as of September 2026 and may have changed.
