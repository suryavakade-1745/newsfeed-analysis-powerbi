# Newsfeed Analysis — Power BI

A Power BI dashboard that analyses newsfeed data to show which sources dominate coverage and how publishing volume trends over time, supporting data-driven media decisions.

<img width="100%" alt="Newsfeed Analysis dashboard" src="https://github.com/user-attachments/assets/bdfa04a2-7f3b-40d0-9db8-346bb267b15c" />


## Business question

Which news sources dominate the feed, and how does article volume change over time?

## Key insights

- **100 articles** analysed from July–August 2024.
- **Business Insider** is the dominant source at **60%** of all articles.
- **Bringatrailer** follows at **10%**, then a long tail of smaller sources (Forbes, DIYphotography, Geeky Gadgets, Android Central and others) at under 5% each.

## Dataset

| Item | Detail |
|---|---|
| Source | Newsfeed dataset of news articles (July – August 2024) |
| Grain | One row per article |
| Main fields | Title, URL, Image URL, Published At, Source Name |

## Approach

1. **Load** – imported the newsfeed data into Power BI Desktop.
2. **Transform (Power Query)** – expanded the nested article records into columns, set data types, and created a published-date column plus a sort-order column so dates display in the right order.
3. **DAX measures** – built dynamic measures for article count and percentage share by source.
4. **Visualise** – built the report page shown above.

| Visual | What it answers |
|---|---|
| Date slicer & date table | Filter and browse by published date |
| URL + image cards | Preview each article with its thumbnail and link |
| KPI card – Count of articles | Total articles in the selected period |
| Line – Articles by published date | Publishing volume over time |
| Line – Articles by source | Ranking of sources by volume |
| Pie – Share by source | Each source's % of total coverage |

## Repository contents

```
newsfeed-analysis-powerbi/
├── README.md
├── Newsfeed Power BI.pbix            # Power BI file
├── Newsfeed Power BI.pdf             # PDF export for quick viewing
└── Newfeeed Analysis Excel.xlsx      # source data (exported from the .pbix)
```

## How to view

- **No Power BI?** Open [Newsfeed Power BI.pdf](Newsfeed%20Power%20BI.pdf).
- **Want the data?** Download [Newfeeed Analysis Excel.xlsx](Newfeeed%20Analysis%20Excel.xlsx).
- **With Power BI Desktop** (free, Windows): download [Newsfeed Power BI.pbix](Newsfeed%20Power%20BI.pbix) and open it — the data loads with it.

## Tools

Power BI Desktop · Power Query · DAX

---

**Surya V Vakade** — SAP FICO · Finance & Analytics
[LinkedIn](https://www.linkedin.com/in/surya-vv) · [GitHub](https://github.com/suryavakade-1745)
