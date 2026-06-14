## 👋 Hello, I'm Yingdong Mao
Welcome to my GitHub page! Here, I share useful code and tools related to option pricing, asset pricing, and portfolio management from my academic projects. Feel free to explore and clone them for your use. If you find these resources helpful, I would greatly appreciate it if you could provide proper citations.

## 👤 Biography
👨‍🏫 Lecturer (Assistant Professor) in Finance at University of Sydney Business School

🎓 PhD in Finance at University of Texas at Dallas | Master in Mathematical Finance at Bentley University

📚 Research Focus: Asset Pricing, Options, and Portfolio Theory

💻 Experienced in Python, R, MATLAB

## 🔬 Research Projects

- 📄 [**Ex-Ante Risk Premia on Earnings Announcements: Evidence from the Options Market**](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4342267) with [Hong Liu](https://apps.olin.wustl.edu/faculty/liuh/), [Xiaoxiao Tang](https://sites.google.com/view/xiaoxiaotang-homepage), and [Guofu Zhou](https://apps.olin.wustl.edu/faculty/zhou/) — **R&R at *Journal of Accounting and Economics***
  + 🔍 Key Contribution: First paper to estimate the ex-ante risk premium on earnings announcements directly from the options market.
  + 📊 Findings: Earnings-announcement risk premia predict both the underlying stock returns and the straddle returns around the announcement.
  + 📈 Innovation: An "EA-managed S&P 500 portfolio" that lifts the Sharpe ratio by ~51% over the unmanaged version.
  + 🧠 **New in this revision:** A novel structural model that explains the Earnings Response Coefficient (ERC) and the Post-Earnings-Announcement Drift (PEAD) within a **single, integrated framework** — closing a long-standing dichotomy in the literature. The model's predictions are confirmed both in simulation and in the data.

- 📈 [**Hedging Corporate Event Risk**](https://drive.google.com/file/d/1CFTNOC7vzK7B1x5FCDE3rwUl3aoq81We/view)
  + 🔧 Methodology: Constructs $RRP^v$, a **novel option-implied measure** of investors' demand to hedge against *scheduled corporate events*, by decomposing the equity-option implied-volatility surface.
  + 📅 Scheduled events the measure captures: Earnings Announcement Days (EAD) and Annual General Meetings (AGM).
  + 📖 Framework: Builds on [Carr and Wu (2020)](https://onlinelibrary.wiley.com/doi/abs/10.1111/jofi.12894) to decompose the implied volatility surface of equity options.
  + 💡 Insight: $RRP^v = \text{variance risk premium} \times \text{hedge ratio}$. Predicts realized returns ahead of the scheduled event.

- 📉 [**Timing the Downside: Managed Portfolios as Cost-Sensitive Classification**](https://github.com/yingdongmao/Multifactor) with [Feng Zhao](https://jindal.utdallas.edu/faculty/feng-zhao/) and [Xiaoxiao Tang](https://sites.google.com/view/xiaoxiaotang-homepage)
  + 🎯 **Framing shift.** The volatility-managed literature treats volatility as the *quantity* of risk to be scaled away. We treat it as a **state variable** (ICAPM-style), describing the investment opportunity set. The question becomes *what is the conditional distribution?*, not *what is the conditional mean?* — volatility predicts the downside state, and more precisely the *probability* of a downside.
  + ⚖️ **Cost-sensitive, fully ex-ante.** The threshold that separates "downside" from "no action" is set by the relative cost of the two errors — holding through a downside vs. cutting before a rally — *estimated in real time* from the forecast conditional tails. Because those costs are valued through the investor's utility, the threshold reflects both predictable tail asymmetry and her risk aversion. No look-ahead.
  + 🪜 **Three layers of performance gain:**
    1. Conditioning on a predicted downside state, even a simple **half-position step-down** beats buy-and-hold.
    2. Scaling the step-down by the predicted *probability* (confidence) of a downside improves performance further.
    3. Because forecasting skill varies across factors and over time, a **skill-weighted multifactor portfolio** — built in the spirit of DeMiguel et al. (2024) — improves performance further still. The investor faces Bayesian model uncertainty but **learns from the market**, especially around recessions and downturns.
  + 💼 **Implementation.** We replicate the nine factors at the individual-stock-holding level (à la DeMiguel et al.); the multifactor portfolio additionally benefits from **trade netting**, giving it a transaction-cost edge over every alternative we considered.
  + 🔒 *Code repository is private; it will be made public once the paper is accepted for publication.*

- 🧮 [**Option-Implied Betas under a Common Lens: Buss–Vilkov vs Kempf–Korn–Saßning, with an Emphasis on the Term Structure**](https://github.com/yingdongmao/OI_BETA) with Chao Gao (Australian National University)
  + 🔬 Places the two leading option-implied beta estimators inside a single decomposition $\beta_i = \rho_{iM}\,\sigma_i/\sigma_M$, and shows that the entire methodological difference reduces to **one object** — a stock-specific implied market correlation (BV) vs. a market-wide constant (KKS).
  + 🧩 **Nesting result.** KKS is the constant-correlation limit of BV in the large-diversification case; the two methods sit on a spectrum of progressively stronger restrictions on the *shape* of the risk-neutral correlation matrix.
  + 📐 **Term structure.** BV carries a name-specific correlation term structure (better when the signal lives in correlations); KKS carries only a market-wide one but **degrades much more gracefully** when long-horizon pairwise-correlation data are unreliable.
  + 📊 **Clean attribution.** Decomposing $\sigma^{IV} = \sigma^{ERV} + \sigma^{VRP}$ additively, the KKS beta admits a clean split into ERV and VRP components sharing the same denominator — useful for per-stock attribution of the beta slope. BV does not, because both its index volatility and its risk-neutral correlation carry their own risk premia.
  + 🔒 *Code repository is private; it will be made public once the paper is accepted for publication.*

## 🎓 Teaching Innovation

- 🎲 [**Trading Games — live multiplayer classroom market simulations**](https://github.com/yingdongmao/trading-game) (FINC3014 *Trading and Dealing in Security Markets*, University of Sydney)
  + Three live multiplayer browser games hosted on a single **zero-dependency Python server**:
    - **Open Cross** — call auction + continuous LOB (Week 2 auction market).
    - **Dealer Floor** — pure dealer market with inventory risk (Week 2 dealer market).
    - **Dealer Pit** — Glosten–Milgrom adverse selection (Week 4 / Week 8 informed trading).
  + Instructor switches modes from an admin console; students join from a **single URL by scanning a QR code**. Real-time projector charts (live supply/demand cross; LOB depth; dealer inventory drift; over-the-session VWAP / P\* trend).
  + **Validated for 120 concurrent players, 0 errors, p95 latency ~25 ms** on a laptop.
  + Feedback from PhD-student testers — including non-finance majors — was that they grasped the basic mechanism of market microstructure within ~10 minutes of play.
  + Built end-to-end with AI assistance. Companion lecture slides integrate the games directly into the live lecture flow.

### 📚 Skills
![Python](https://img.shields.io/badge/Python-3.8-blue) ![R](https://img.shields.io/badge/R-4.0.2-lightblue)
![LaTeX](https://img.shields.io/badge/LaTeX-Professional-orange)

🔗 [Google Scholar](https://scholar.google.com/citations?user=j0c2PTwAAAAJ&hl=en) | [Website](https://sites.google.com/view/yingdong-mao/home) | [LinkedIn](https://www.linkedin.com/in/yingdong-mao-022a45a1)
