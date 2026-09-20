# Power BI Dashboard Specification
## InvestForChange Podcast Analytics

### Data Sources

| Source | Connector | Refresh |
|--------|-----------|--------|
| GA4 | BigQuery connector | Daily |
| Spotify for Podcasters | API / CSV export | Weekly |
| Apple Podcasts Analytics | CSV manual export | Weekly |
| Google Sheets (social metrics) | Google Sheets connector | Daily |

---

### Page 1: Audience Overview

- **KPI cards:** Total listeners | Total plays | Unique listeners | Avg episode plays
- **Bar chart:** Episode reach by platform (Spotify / Apple / Web / Other)
- **Map:** Listener geography — South Africa provinces (choropleth)
- **Line chart:** Weekly listener growth trendline (cumulative)

---

### Page 2: Episode Performance

- **Table:** Episode | Plays | Avg duration (sec) | Completion % | Shares
- **Bar chart:** Completion rate % per episode
- **Scatter:** Avg listen duration vs. episode number
- **Heatmap (matrix):** Drop-off point buckets (0–25%, 25–50%, 50–75%, 75–100%)

---

### Page 3: Conversion Funnel

- **Funnel chart:** Listeners → Website visits → Whitepaper downloads → Newsletter signups
- **Line chart:** Weekly whitepaper downloads over time
- **Bar chart:** GTM conversion events by source (social / direct / organic)

---

### Page 4: Policy Impact Tracker

- **KPI card:** Total whitepaper downloads
- **Line chart:** Downloads over time by episode reference
- **Word cloud / bar:** Social hashtag mentions (#InvestForChange)
- **Counter:** Press coverage articles
- **Timeline:** Government engagement events

---

### Season 1 KPI Targets

| Metric | Target |
|--------|--------|
| Total listeners | 10,000 |
| Avg completion rate | > 60% |
| Whitepaper downloads | 2,000 |
| Newsletter signups | 1,500 |
| Press mentions | 20 |

---

### Refresh & Access

- Daily auto-refresh via Power BI Service
- Requires Power BI Pro or Premium Per User licence
- Shared workspace: `InvestForChange Analytics`
- Row-level security: not required (public podcast data)
