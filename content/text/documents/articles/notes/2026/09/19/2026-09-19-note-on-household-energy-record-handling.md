---
title: "Household energy record handling"
description: "How household energy readings are recorded, compared and protected; the facts themselves are observation records in this section."
date-created: 2026-09-19
date-observed: 2026-09-05
type: note
name: 2026-09-19-note-on-household-energy-record-handling
status: draft
keywords:
  - household-energy
  - utility-tariff
  - net-metering
---

# Household energy record handling

The dated facts from the September 5 household-energy study (unit conversions, the South Dakota LIHEAP range, Public Law 119-21, PVWatts, PV EROI and storage, renewable-energy certificates) are observation records in [`data/records/observation-records/`](../../../../../../../../data/records/observation-records/), each with its source and date. This note states how a household's own readings are handled.

## What a household record keeps

- Electricity use and on-site generation are separate quantities. A utility statement, a meter reading and an inverter or manufacturer-portal export are separate witnesses. A disagreement between them is recorded as a discrepancy with its signed amount and both witnesses.
- A tariff is local and dated. Its record holds the utility, the rate-schedule name, the tiered price per kWh, any net-metering credit and rollover rule, the source URL and the date it was read.
- The physical resources are grid electricity (kWh), distributed-generation credit (net-metered kWh), propane, diesel or heating oil, and cordwood. Each has its own delivery rail and unit of account.
- A billing-period record holds the period start and end, the household identifier or a local substitute, the source and observation date, the quantities and units, and the tariff in effect.
- Statement layout is source data. The column mapping and date format used to read a statement are kept with it and named per utility statement, not per utility.
- An unparseable row, or a statement total that differs from its listed charges, is an unresolved input.
- A fuel or commodity without a dated, cited price is unpriced.

## Handling

- Household readings are sensitive. They stay local or in the household's governed store.
- A household's choice not to optimize is a valid state of the record.
- A computation compares observations, converts a declared quantity or summarizes evidence. Ownership, interconnection, equipment control, utility negotiation and household decisions belong to the household and its consent.
- A PV yield projection is an estimate that cites its location, dataset, system size and performance assumption. Panel telemetry is the measurement.
- Software layers describing solar, battery, credit or exchange arrangements are records of that software. A household's system, permission to connect, battery, saleable credit or exchange agreement each need their own physical, legal and consent evidence.

## Sources

- U.S. Energy Information Administration, *Monthly Energy Review*, Appendix A conversion factors: <https://www.eia.gov/totalenergy/data/monthly/pdf/sec12.pdf>
- National Renewable Energy Laboratory, PVWatts Calculator: <https://pvwatts.nrel.gov/>
- U.S. Department of Health and Human Services, LIHEAP: <https://www.acf.hhs.gov/ocs/low-income-home-energy-assistance-program-liheap>
- Raugei, Leccisi and Fthenakis (2020), *Energy Technology*: <https://doi.org/10.1002/ente.201901146>
