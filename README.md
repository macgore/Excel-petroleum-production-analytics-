# Excel-petroleum-production-analytics-
Excel based production surveillance and executive dashboard for a simulated 120 well oil & gas portfolio  pivot table style analytics, KPI tracking, and data driven optimization recommendations across field, reservoir, and pump type performance.

Dataset

120 producing wells across:
- Fields: Alpha, Bravo, Charlie
- Reservoirs: Sand A, Sand B, Carbonate C
- Pump types: ESP, Rod Pump, Gas Lift
- Completions: Vertical, Deviated, Horizontal

15 columns per well including oil/gas/water rates, water cut, pressure, downtime, and operating cost.

Workbook structure

- Dashboard — KPI cards, Top 10 / Bottom 10 wells by oil rate, interactive filters
- Raw_Data — full 120-well dataset as an Excel Table
- Field Summary / PumpType Summary / Field Pump Summary — pivot-style breakdowns built with `SUMIF`, `AVERAGEIF`, `SUMIFS`, `AVERAGEIFS`
- KPIs — total oil/gas, average water cut, average pressure, well counts, intervention flags
- Charts — Oil by Field, Well Status distribution, Oil by Pump Type, Pressure by Field, Water Cut by Field
  
Key findings

- Total portfolio production: 49,952 bbl/day oil, 49,793 Mscf/day gas, at 30.6% average water cut
- Alpha field leads production (19,121 bbl/day) with the highest reservoir pressure and lowest water cut
- ESP wells outproduce Rod Pump wells by ~2.5x  (559 vs. 224 bbl/day average) — all top 10 wells run ESP, 8 of the bottom 10 run Rod Pump
- 20 wells (16.7%) meet the intervention criteria: water cut above 50% or downtime above 25 hours
- Bravo field carries the highest average water cut (33.7%) of the three fields

Full analysis and recommendations are in `Production_Analytics_Report`.

 Skills demonstrated

- PivotTable-equivalent aggregation using `SUMIF`/`SUMIFS`/`AVERAGEIF`/`AVERAGEIFS`/`COUNTIF`
- KPI calculation with `INDEX/MATCH`, `LARGE`/`SMALL`, and `SUMPRODUCT` for multi-condition flags
- Native Excel chart construction (bar, column, line, pie)
- Executive dashboard layout and design
- Data driven engineering recommendations
