# 1. Background

[← Back to the summary](./README.md)

## How a new power plant gets connected

Every solar farm, wind farm, or big battery that wants to sell electricity has to plug into the power grid: the network of high-voltage lines that carries electricity from power plants to homes and businesses.

Before it can plug in, the grid operator has to study what the new plant will do to the rest of the system. Will a line overload? Does a substation need upgrading? Who pays for that?

Projects wait for those studies in a line called the **interconnection queue**. In this study I mostly just call it **the waiting line**.

The line is long, and it is slow:

- Lawrence Berkeley National Laboratory found that, of the projects that joined the line between 2000 and 2020, only **13% were built and running** by the end of 2025. About **75% dropped out**.
- For projects that did finish in 2025, the typical wait from joining the line to turning on was **more than five years**.
- On a recent episode of the *Catalyst* podcast, Tim Hade estimated that getting through the line takes about **four years in Texas**, **six years in the Mid-Atlantic**, and **up to nine years in California**. ([Latitude Media](https://www.latitudemedia.com/news/catalyst-why-ci-storage-is-finally-taking-off/))

## What "the Berkeley study" is

Lawrence Berkeley National Laboratory, a U.S. Department of Energy lab, publishes a yearly report called [*Queued Up*](https://emp.lbl.gov/queues). It gathers the waiting lines from grid operators and utilities across the country into one public dataset.

The [2026 edition](https://emp.lbl.gov/publications/queued-2026-edition-characteristics) covers data through the end of 2025. It found:

- About **8,200 active requests** to connect.
- About **1,312 gigawatts of power plants** and **749 gigawatts of batteries**. Together that is about **2.06 terawatts**.
- About **549 gigawatts** already have a signed or draft agreement with the grid and still aren't running.

Headlines often round this to "more than 2 terawatts stuck." Earlier editions put it at about 2.3 terawatts. The number moves: on 8 September 2026, the live tracker [interconnection.fyi](https://www.interconnection.fyi) showed about **1.92 terawatts** still active.

### How big is a terawatt?

| Unit | Equals | Rough sense of scale |
| --- | --- | --- |
| 1 megawatt (MW) | 1,000 kilowatts | Enough to power a few hundred U.S. homes |
| 1 gigawatt (GW) | 1,000 megawatts | A large power plant, or one of the biggest AI data center campuses |
| 1 terawatt (TW) | 1,000 gigawatts | All the power plants running in the U.S. today add up to about 1.3 TW |

So 2 terawatts waiting in line is a very large amount of power.

## Why data centers care

Data centers, especially the ones built for AI, use enormous amounts of electricity, and they want it fast. A large AI campus can need hundreds of megawatts, or more than a gigawatt.

Those data centers face the same problem as power plants: connecting a big new electricity user to the grid can also take years.

Some companies have found a way around it: **build the data center right next to its own power source** and connect the two directly. Examples:

- **Gas:** Microsoft and Chevron announced a 20-year deal for gas power plants built next to a data center in West Texas, a project called Kilby. ([Chevron](https://www.chevron.com/newsroom/2026/q2/chevron-signs-20-year-power-agreement-with-microsoft-for-west-texas-data-center))
- **Solar, wind, and batteries:** Google and Intersect Power built a project in Haskell County, Texas, with a large solar farm and battery next to a Google data center.

## The question this study asks

If 2 terawatts of mostly clean power is stuck in line, and data centers are desperate for power, **why aren't more data centers just building next to those stuck projects?**

That's the reason I built [WattConnector](https://wattconnector.munjr.com/), a free tool that maps U.S. data centers against nearby solar, wind, and battery projects and ranks possible pairs. The idea, from its [motivation page](https://wattconnector.munjr.com/motivation/):

- The **solar or wind developer** gets a guaranteed buyer without waiting years in line.
- The **data center** gets clean power years sooner.

This study tests whether that idea holds up when you look at real projects.

## What "worth it" means here

To judge whether a pairing is worth it, I compared it to the expensive option that's already happening: **building gas power plants next to the data center**, as in the Microsoft and Chevron deal.

Public estimates of that project, discussed on the *Energy Empire* podcast in August 2026 (about $9 billion for about 2.67 gigawatts), work out to roughly **$650,000 per megawatt per year** just to pay back the cost of building it, before paying for fuel. An analyst at TD Securities put the all-in cost of its electricity at about **$150 per megawatt-hour**.

A megawatt-hour is one megawatt of power used for one hour. It's the unit electricity is usually priced in.

That gives a simple test: **can a solar or wind farm next door, with batteries, supply a data center reliably for less than that?**

The catch is the word "reliably." Data centers run 24 hours a day. Solar stops at sunset. Wind comes and goes. Any answer has to deal with the night.

---

[Next: Finding and checking possible pairs →](./02-finding-and-checking-pairs.md)
