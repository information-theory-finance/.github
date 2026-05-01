<div align="center">

<pre>
██╗████████╗███████╗
██║╚══██╔══╝██╔════╝
██║   ██║   █████╗  
██║   ██║   ██╔══╝  
██║   ██║   ██║     
╚═╝   ╚═╝   ╚═╝     
</pre>

**Information Theory × Finance**

<br/>

[![Author](https://img.shields.io/badge/Author-Pranava%20BA-C9A84C?style=flat-square)](https://github.com/pranava-ba)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-pranava--ba-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/pranava-ba-aa61a4306/)
[![Location](https://img.shields.io/badge/Chennai-India-0055A5?style=flat-square)]()

[![Docs](https://img.shields.io/badge/📖%20Master%20Docs-itf.readthedocs.io-1ABC9C?style=for-the-badge&logo=readthedocs&logoColor=white)](https://itf.readthedocs.io/en/latest/)

<br/>

*A series of interactive apps exploring information-theoretic concepts — entropy, mutual information,*  
*transfer entropy, KL divergence — and their concrete applications to NSE financial data.*

</div>

<br/>

---

## What This Is

Each project in this series is a two-page Streamlit app:

| Page | Content |
|------|---------|
| **Theory** | Mathematical foundations of the concept, interactive visualisations on synthetic data, formula derivations |
| **Finance** | The same concept applied to live NSE equity and commodity data, self-updating daily |

All projects share a unified dark navy / amber theme, the same DuckDB-backed NSE data store, and a common ReadTheDocs documentation structure.

---

## Projects

<!-- Add a row per project as it is published. -->

| Project | Concept | Live Demo | Docs |
|---------|---------|-----------|------|
| 🔜 *Shannon Entropy* | Measuring uncertainty in return distributions | — | — |
| 🔜 *Mutual Information* | Dependence between asset returns beyond correlation | — | — |
| 🔜 *KL Divergence* | Comparing return distributions across regimes | — | — |
| 🔜 *Transfer Entropy* | Directional information flow between assets | — | — |

*This table is updated each time a new project is added to the organisation.*

---

## Infrastructure Repositories

| Repository | Purpose |
|------------|---------|
| [`nse-data-store`](../../nse-data-store) | Shared DuckDB data store. NSE EOD OHLCV data for NIFTY 50, RELIANCE, INFY, HDFCBANK, GOLDBEES. Self-updating via yfinance. |
| [`itf-theme`](../../itf-theme) | Shared Streamlit `config.toml`, `theme.py` colour constants, and Plotly layout base. The single source of truth for visual consistency. |
| [`docs-master`](../../docs-master) | Master ReadTheDocs hub. Aggregates all project documentation via Sphinx `intersphinx`. |

---

## Stack

<details>
<summary><strong>Tools and Libraries</strong></summary>
<br/>

| Layer | Technology |
|-------|-----------|
| **Frontend** | Streamlit — two-page app per project, wide layout |
| **Charts** | Plotly — all visualisations share a common dark navy theme |
| **Data** | DuckDB — local OHLCV store, NSE data via yfinance |
| **Math** | NumPy, SciPy — implementations in isolated `math_core.py` modules |
| **Docs** | Sphinx + sphinx-rtd-theme + custom CSS, hosted on ReadTheDocs |
| **Hosting** | Streamlit Community Cloud (one app per project) |
| **Data Source** | NSE India via yfinance — EOD OHLCV, auto-updated daily |

</details>

---

## Intellectual Thread

The projects in this series are not isolated tools. They follow a deliberate progression:

```
Entropy (uncertainty in one asset)
    ↓
Mutual Information (shared uncertainty between two assets)
    ↓
KL Divergence (how distributions shift across regimes)
    ↓
Transfer Entropy (directed information flow — who leads whom)
    ↓
Channel Capacity (limits of predictability in financial time series)
```

Each concept builds on the previous. The same NSE tickers appear throughout,
so results are comparable across projects.

---

<div align="center">

**Pranava BA** · Chennai, India · © 2025–2026  
[github.com/pranava-ba](https://github.com/pranava-ba) · [linkedin.com/in/pranava-ba-aa61a4306](https://linkedin.com/in/pranava-ba-aa61a4306/)

</div>
