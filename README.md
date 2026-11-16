# GLP Chart US GLP-1 Cash Prices

GLP Chart US GLP-1 Cash Prices is an open dataset of the cash prices that US online programs charge for GLP-1 medications (semaglutide and tirzepatide, brand-name and compounded), read from each program's own published pricing page. Compiled by John Samaras, price analyst, GLP Chart (https://glpchart.com), Bolvon Pty Ltd.

Headline figure: the median US online GLP-1 program charged US$299 a month in cash in October 2026 (GLP Chart GLP-1 Cash Price Index, November 2026 release).

## Files
- `glp-chart-price-history.csv`: one row per program per check date: `date`, `program_slug`, `program_name`, `headline_maintenance_monthly_usd` (the monthly price at the dose a person stays on, all required fees included). From 25 May to 9 November 2026, weekly. A blank price means the program was not listed or not priced on that date.
- `glp-chart-price-index-2026-11.csv`: the November 2026 edition of the GLP Chart GLP-1 Cash Price Index (October 2026 data): the median all-in monthly price and the cheapest verified routes, each with its source.

## Method
- Each price is read from the program's own website, daily since 12 Nov 2026 (weekly before), and dated with the day it was read.
- "All-in" counts every required fee (membership, consult, medication) for one month at the maintenance dose.
- A program with a yearly membership shows its monthly drug price with the membership named beside it.
- Compounded semaglutide and tirzepatide are made by pharmacies and are not FDA-approved; they are not Wegovy, Ozempic, Zepbound or Mounjaro.
- Full method: https://glpchart.com/methodology/ and https://glpchart.com/how-we-check-prices/

## Coverage
United States. 25 May 2026 to 9 November 2026 in this version. A new version is published each month; the live data is at https://glpchart.com/data/

## Licence and citation
Creative Commons Attribution 4.0 (CC BY 4.0).

Cite as: Samaras J. GLP Chart US GLP-1 Cash Prices [dataset]. GLP Chart; 2026. https://doi.org/10.5281/zenodo.24245067

```bibtex
@dataset{samaras_glp_chart_us_glp1_cash_prices_2026,
  author    = {Samaras, John},
  title     = {GLP Chart US GLP-1 Cash Prices},
  year      = {2026},
  publisher = {GLP Chart},
  doi       = {10.5281/zenodo.24245067},
  url       = {https://doi.org/10.5281/zenodo.24245067}
}
```

## Copies
- Zenodo: https://doi.org/10.5281/zenodo.24245067
- Hugging Face: https://huggingface.co/datasets/glpchart/us-glp1-cash-prices
- Kaggle: https://www.kaggle.com/datasets/johns1230/us-glp-1-cash-prices-monthly
- Live data and API: https://glpchart.com/data/

## Data dictionary
| File | Column | Meaning |
|---|---|---|
| glp-chart-price-history.csv | date | Day the price was read (YYYY-MM-DD) |
| glp-chart-price-history.csv | program_slug | Stable short id for the program |
| glp-chart-price-history.csv | program_name | Program name as shown on GLP Chart |
| glp-chart-price-history.csv | headline_maintenance_monthly_usd | All-in monthly cash price at the maintenance dose, US dollars; blank if not listed or not priced that day |
| glp-chart-price-index-2026-11.csv | program, drug, form | The route the row describes |
| glp-chart-price-index-2026-11.csv | monthly_price_usd | Monthly cash price, US dollars |
| glp-chart-price-index-2026-11.csv | plan, last_verified, source_url | What the figure is, when it was checked and where |

## Notes
Prices only. Nothing here is medical advice. Some listed programs pay GLP Chart when a reader signs up.
