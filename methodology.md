# Methodology and Data Notes

This page explains the calculations used in the submitted Excel workbook. It accompanies Part 1 and documents the existing work.

## Period and units

The analysis covers Target’s **fiscal years 2020–2024**. The `Financial Data` sheet also contains 2019 balances so that 2020 turnover ratios can use an average of beginning and ending balances. Financial statement amounts are in **$ millions**. Timing measures use **365 days**. Reported ratios are rounded to two decimal places; the workbook retains greater precision.

A filing published in 2025 can contain fiscal 2024 results. The report’s reference to Target’s 2025 Form 10-K does not extend the analysis to fiscal 2025.

## Efficiency calculations

Average balance means the arithmetic mean of the previous and current fiscal year-end balances.

| Measure | Formula used in the workbook |
| --- | --- |
| Total asset turnover | Sales / average total assets |
| Inventory turnover | Cost of sales / average inventory |
| Days inventory outstanding | 365 / inventory turnover |
| Accounts receivable turnover | Sales / average other current assets, used as a receivables proxy |
| Average collection period | 365 / accounts receivable turnover |
| Accounts payable turnover | Cost of sales / average accounts payable |
| Average payment period | 365 / accounts payable turnover |
| Operating cycle | Days inventory outstanding + average collection period |
| Cash conversion cycle | Operating cycle − average payment period |

The `Efficiency` sheet links its turnover calculations to the `Financial Data` sheet. Other current assets are not a separately identified accounts receivable balance. The receivables turnover and collection period are estimates based on that proxy. The operating and cash conversion cycles inherit this limitation.

For 2024, the rounded timing values are 58.75 inventory days, 6.44 collection days, and 60.00 payment days, giving a cash conversion cycle of approximately **5.19 days**.

## Asset turnover in efficiency and DuPont analysis

The `Efficiency` sheet divides sales by **average total assets**, producing 2024 asset turnover of **1.88**. The `DuPont` sheet divides sales by **year-end total assets**, producing **1.84**. These values use different denominators and should be interpreted within their respective sections.

## Reading the original report alongside the workbook

The repository preserves the four supplied files. The README uses the workbook values and fiscal-year labels when the report’s narrative differs:

| Item | Original report narrative | Workbook value used in README |
| --- | --- | --- |
| 2024 sales | $107,588 million | $106,566 million; $107,588 million belongs to 2022 |
| 2021 operating income | $8,846 million | $8,946 million |
| Operating cycle of 65.18 days | Labeled 2025 in the efficiency paragraph | Fiscal 2024 |

## Source references

The following links are transcribed from the report’s reference list:

- [Target Form 10-K, fiscal year ended February 1, 2020](https://www.sec.gov/Archives/edgar/data/27419/000002741920000008/tgt-20200201.htm) — includes fiscal 2019 balances used for averaging.
- [Target Form 10-K, fiscal year ended January 30, 2021](https://www.sec.gov/Archives/edgar/data/27419/000002741921000010/tgt-20210130.htm).
- [Target Form 10-K, fiscal year ended January 29, 2022](https://www.sec.gov/Archives/edgar/data/27419/000002741922000007/tgt-20220129.htm).
- [Target Form 10-K, fiscal year ended January 28, 2023](https://www.sec.gov/Archives/edgar/data/27419/000002741923000015/tgt-20230128.htm).
- [Target Form 10-K, fiscal year ended February 3, 2024](https://www.sec.gov/Archives/edgar/data/27419/000002741924000032/tgt-20240203.htm).
- [Target Form 10-K, fiscal year ended February 1, 2025](https://www.sec.gov/Archives/edgar/data/27419/000002741925000018/tgt-20250201.htm).
- [Yahoo Finance historical prices for Target](https://finance.yahoo.com/quote/TGT/history/) — used by the group for market ratios.

