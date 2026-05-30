# IPL Cricket Analytics 🏏

An end-to-end data analytics project built during my CodeAlpha Data Analytics Internship.
I picked cricket because I actually watch it — and honestly that made the analysis way more fun to build.

---

## What this project does

Takes IPL data from 2008 to 2024 and tries to answer questions that actually matter as a cricket fan:

- Which team has genuinely dominated over the years?
- Does winning the toss actually help or is it just a coin flip?
- Who are the real all-time greats with the bat and ball?
- How has scoring changed season by season?
- What separates elite IPL batters from just good ones?

---

## Tasks covered

| Task                        | What I did                                                                 |
| --------------------------- | -------------------------------------------------------------------------- |
| Task 1 — Web Scraping       | Scraped live IPL 2026 batting stats from ESPN Cricinfo using BeautifulSoup |
| Task 2 — EDA                | Explored 900+ matches across 17 seasons, answered 7 analytical questions   |
| Task 3 — Data Visualization | Built 8 charts using Matplotlib and Seaborn                                |

---

## Charts built

1. Top 10 teams by all-time wins
2. Toss analysis — does it actually matter?
3. Top 10 run scorers of all time
4. Top 10 wicket takers of all time
5. Season-wise total runs trend (2008–2024)
6. Scoring rate by match phase (Powerplay / Middle / Death)
7. Win margin distribution — batting first vs chasing
8. IPL 2026 Strike Rate vs Average scatter (using scraped data)

---

## Dataset sources

- **Historical data (2008–2024):** [IPL Complete Dataset — Kaggle](https://www.kaggle.com/datasets/patrickb1912/ipl-complete-dataset-20082020)
- **Live 2026 stats:** Scraped from [ESPN Cricinfo](https://www.espncricinfo.com/records/tournament/batting-most-runs-career/indian-premier-league-2026-17740)

---

## Tech stack

```
Python 3.x
├── requests          — HTTP requests for scraping
├── BeautifulSoup4    — HTML parsing
├── pandas            — data loading, cleaning, analysis
├── numpy             — numerical operations
├── matplotlib        — base visualizations
└── seaborn           — statistical charts
```

---

## How to run this

**1. Clone the repo**

```bash
git clone https://github.com/pythonom/CodeAlpha_IPLCricketAnalytics
cd CodeAlpha_IPLCricketAnalytics
```

**2. Install dependencies**

```bash
pip install requests beautifulsoup4 pandas numpy matplotlib seaborn lxml
```

**3. Download the Kaggle dataset**

Go to the Kaggle link above, download and extract — you'll get `matches.csv` and `deliveries.csv`.
Place both files in the root of this folder.

**4. Run the notebook**

```bash
jupyter notebook IPL_Cricket_Analytics.ipynb
```

Run all cells top to bottom. The scraping cell has a fallback built in, so it works even if ESPN Cricinfo blocks the request.

---

## Key findings

- **MI and CSK** dominate all-time win counts by a significant margin
- Toss advantage is **statistically weak** — toss winners win only ~52% of the time, barely above random
- Death overs scoring rate is notably higher than middle overs, confirming the tactical shift in modern T20

---

## Repo structure

```
CodeAlpha_IPLCricketAnalytics/
├── IPL_Cricket_Analytics.ipynb   ← main notebook
├── ipl_2026_live_batting.csv     ← scraped during runtime
├── chart1_team_wins.png
├── chart2_toss_analysis.png
├── chart3_top_batters.png
├── chart4_top_bowlers.png
├── chart5_season_runs.png
├── chart6_match_phases.png
├── chart7_win_margins.png
├── chart8_ipl2026_scatter.png
└── README.md
```

---

## Internship

Built as part of the **CodeAlpha Data Analytics Internship**
[www.codealpha.tech](https://www.codealpha.tech)

---

_If you find something interesting in the data or want to build on this, feel free to fork it._
