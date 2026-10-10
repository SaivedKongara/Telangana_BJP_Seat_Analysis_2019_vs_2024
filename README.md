# Telangana BJP Seat Analysis: 2019 vs 2024

Which of Telangana's 17 Lok Sabha seats should BJP put more effort into next time, and where would that effort likely be wasted? This project compares the 2019 and 2024 results seat by seat and ends in one decision per seat.

## Data
- Constituency-wise detailed results for the 2019 and 2024 Lok Sabha elections, from the Election Commission of India (17 seats in Telangana).
- The first two sheets hold the raw results. Every analysis sheet is built from them with live Excel formulas (VLOOKUP, IFS), with no hard-coded values.

## Method
1. **Seat grade:** average of BJP's margin (%) in 2019 and 2024. 10% or more is Strong Hold, 5-10% Average Hold, -5% to 5% Weak Hold, below -5% Very Vulnerable Hold.
2. **Conversion:** BJP's vote-share swing divided by the turnout swing. Above 5 is High (real movement, mobilise voters), 3-5 is Moderate (strengthen the existing base), below 3 is Low (gain mostly from higher turnout).
3. **Candidate vs seat:** the same candidate who won both years is a Strong Candidate Face. A different candidate who won both is Strong Party Presence. A new candidate with a rising vote share is a Potential Candidate (retain). Seats are Strong (won both), Swing (won one) or Weak (lost both).
4. **Decision:** strong candidate or party presence gives Invest & Maintain. A swing seat with High or Moderate conversion gives Invest to Flip. A weak seat with High conversion gives Mobilize Aggressively. Everything else is Deprioritize.

Full reasoning is in the [methodology document](docs/Telangana_BJP_Seat_Analysis_Methodology.docx) (Word file, download to read).

## Results

| Decision | Seats |
|---|---|
| Invest & Maintain (4) | Adilabad, Karimnagar, Nizamabad, Secunderabad |
| Invest to Flip (3) | Medak, Malkajgiri, Chevella |
| Mobilize Aggressively (4) | Peddapalle, Nalgonda, Bhongir, Khammam |
| Deprioritize (6) | Zahirabad, Hyderabad, Mahbubnagar, Nagarkurnool, Warangal, Mahabubabad |

- **Malkajgiri** shows the strongest real shift: BJP's vote share went from 19.5% to 51.6% while turnout rose only 1.7 points.
- **Karimnagar** is the opposite: turnout rose 3.6 points but BJP's vote share moved only 1.3 points.

## Limitations
- Seat grades use a simple average of two margins, not a weighted one, so they understate recent momentum. Medak and Chevella were BJP wins in 2024 but grade as Very Vulnerable Hold because of the 2019 losses. A recency-weighted version is the natural next step.
- "Hold" describes BJP's average standing and also appears for seats BJP lost both years.
- The conversion ratio becomes unstable when the turnout swing is very small (Nalgonda: turnout +1.0 point gives a ratio of 12.65).
- Candidate rating only checks whether the candidate stayed the same. It does not measure personal popularity.
- The analysis describes past results. It is not a prediction.

## Repository
```
analysis/Telangana_BJP_Seat_Analysis_2019_vs_2024.xlsx
docs/Telangana_BJP_Seat_Analysis_Methodology.docx
```
The workbook has 6 sheets: 2024 results, 2019 results, seat grading, turnout analysis, candidate rating and decision. Open it in Excel 2019 or Microsoft 365, since it uses the IFS function.

## Disclaimer
An academic analysis of public data, written from one party's perspective as an exercise. No political affiliation or endorsement is implied.

## Author
Saived Kongara, BBA, IBS Hyderabad (ICFAI)
LinkedIn: linkedin.com/in/ksaived
