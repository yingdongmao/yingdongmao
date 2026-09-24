## 👋 Hello, I'm Yingdong Mao
Welcome to my GitHub page! Here, I share useful code and tools related to option pricing, asset pricing, and portfolio management from my academic projects. Feel free to explore and clone them for your use. If you find these resources helpful, I would greatly appreciate it if you could provide proper citations.

## 👤 Biography
👨‍🏫 Lecturer (Assistant Professor) in Finance at University of Sydney Business School

🎓 PhD in Finance at University of Texas at Dallas | Master in Mathematical Finance at Bentley University

📚 Research Focus: Asset Pricing, Options, and Portfolio Theory

💻 Experienced in Python, R, MATLAB

## 🔬 Research Projects

- 📄 [**Ex-Ante Risk Premia on Earnings Announcements: Evidence from the Options Market**](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4342267) with [Hong Liu](https://apps.olin.wustl.edu/faculty/liuh/), [Xiaoxiao Tang](https://sites.google.com/view/xiaoxiaotang-homepage), and [Guofu Zhou](https://apps.olin.wustl.edu/faculty/zhou/) — **R&R at *Journal of Accounting and Economics***
  + 🔍 **Key contribution.** The first *firm-level* estimates of the ex-ante risk premium on an individual earnings announcement, recovered from the prices of the firm's own short-dated equity options.
  + 📊 **Magnitude.** The premium averages **11 basis points per trading day** across 6,306 S&P 500 announcements, rises with analyst forecast dispersion and idiosyncratic volatility, and identifies in advance the announcements on which selling volatility pays.
  + 🧠 **Structural model.** A three-period Epstein–Zin model in which the announcement resolves only *part* of the firm's uncertainty. The premium prices the anticipated announcement jump; the uncertainty that *survives* the announcement compresses the announcement-window response and defers it into the drift — putting the **earnings response coefficient** and **post-earnings-announcement drift** in one framework.
  + 📈 **Test.** Holding residual uncertainty fixed, a one-standard-deviation higher premium raises the ERC by **1.25 on a base of 3.8**, and PEAD is concentrated among the announcements the premium flags in advance.

- 🧮 [**The Term Structure of Beta**](https://github.com/yingdongmao/OI_BETA) with Chao Gao (Australian National University)
  + 🔬 **Four estimators, one comparison.** Option-implied betas for S&P 500 stocks from four identifying restrictions: Kempf–Korn–Saßning, Buss–Vilkov, a **premium-ratio beta** that strips announcement and idiosyncratic variance out of implied variance, and a **regression-based beta** identified from the co-movement of stock and index implied variances.
  + 📉 **The slope is priced.** For all four, the slope of the term structure (91-day minus 30-day beta) predicts *lower* returns next month: a one-standard-deviation higher slope lowers the next month's return by **19 to 30 basis points**.
  + 🧪 **Not a repackaged anomaly.** For the two new estimators the slope premium survives the stock's own implied-volatility slope and its earnings-announcement component, and is not explained by idiosyncratic volatility, co-movement with common idiosyncratic variance, horizon bias, or mutual-fund demand.
  + 🌏 **Term-structure economics.** Implied *systematic* variance departs from the expectations hypothesis by more than total implied variance, and the premium is larger in recessions — consistent with prices of market risk that decline with horizon.
  + 🔒 *Code repository is private; it will be made public once the paper is accepted for publication.*

- 📉 [**What Does Volatility Forecast? Downside States and Factor Timing**](https://github.com/yingdongmao/Multifactor) with [Xiaoxiao Tang](https://sites.google.com/view/xiaoxiaotang-homepage) and [Feng Zhao](https://jindal.utdallas.edu/faculty/feng-zhao/)
  + 🎯 **Framing shift.** The volatility-managed literature treats volatility as the *quantity* of risk to be scaled away. We treat it as a **state variable** (ICAPM-style) describing the investment opportunity set. Volatility predicts factor *means* weakly, but the *downside state* and the *tail magnitude* strongly — so the question becomes *what is the conditional distribution?*, not *what is the conditional mean?*
  + ⚖️ **Cost-sensitive, fully ex-ante.** The threshold separating "downside" from "no action" is set by the relative cost of the two errors — holding through a downside vs. cutting before a rally — *estimated in real time* from the forecast conditional tails and valued through the investor's utility, so it reflects both predictable tail asymmetry and risk aversion. No look-ahead.
  + 🪜 **Three layers of performance gain:**
    1. Conditioning on a predicted downside state, even a simple **fixed cut** beats buy-and-hold.
    2. Scaling the cut by the predicted *probability* (confidence) of a downside improves performance further.
    3. Because forecasting skill varies across factors and over time, a **skill-weighted multifactor portfolio** — in the spirit of DeMiguel et al. (2024) — improves performance further still.
  + 📊 **Result.** Sharpe ratios rise for **all nine** major equity factors, and the equal-weight nine-factor portfolio goes from **1.26 to 1.74**.
  + 💼 **Implementation.** The rule never scales factor exposure *above* the unmanaged level, so it runs with lower deployment and turnover than volatility-managed and conditional mean–variance alternatives. We replicate the nine factors at the individual-stock-holding level (à la DeMiguel et al.); the multifactor portfolio additionally benefits from **trade netting**.
  + 🔒 *Code repository is private; it will be made public once the paper is accepted for publication.*

- 📈 **Price of Hedging Corporate Event Risk**
  + 🔧 **Measure.** Constructs the **Hedging Premium** $HP^{v}$, an option-implied, firm-level *cost of hedging* scheduled corporate event risk: the price of a unit volatility hedge (the variance risk premium) times the quantity needed to immunize a stock position (the stock's elasticity to implied volatility).
  + 📅 **Behaviour around events.** Estimated daily from the implied-volatility surface for S&P 500 firms, 1996–2024, the cost of hedging **rises into earnings announcements and falls once the news is out**, and stays flat around matched non-events and the market-wide FOMC placebo.
  + 📖 **Framework.** Builds on [Carr and Wu (2020)](https://onlinelibrary.wiley.com/doi/abs/10.1111/jofi.12894) to decompose the implied volatility surface of equity options.
  + 💡 **Result.** Both components forecast the size of the realized announcement move; the pre-event run-up is driven by the *price* of volatility insurance rather than the quantity hedged.

- ⚡ **Inelastic Hedging Demand and Intraday Momentum** with Taeyoung Park (UT Dallas) and [Feng Zhao](https://jindal.utdallas.edu/faculty/feng-zhao/)
  + 📐 **The boundary.** Delta-neutral hedging of a short-gamma book loses with the *square* of the move. The **gamma–theta breakeven range (GTBR)** is the move at which gamma loss equals theta income; beyond it, hedgers' demand for the underlying turns **inelastic**.
  + 📊 **Finding.** Using option market makers' gamma inventory in S&P 500 stocks, 2007–2022, the sign of the dealers' book predicts the **last half hour** of the underlying on days that breached the GTBR: a short-gamma book *continues* the move, a long-gamma book *damps* it. Inside the range the effect is about a third as large and insignificant.
  + 🕒 **Where and when.** The gap opens exactly at the boundary, has the same sign for up and down moves, and grows with the depth of the book. On breach days market makers do not buy back options — the public is a net buyer of gamma from them — so the adjustment is made **in the stock**.

- 🔗 **Where Uncertainty Enters the Supply Chain: Network Position and the Implied-Volatility Surface** *(work in progress)*
  + 🧭 **Idea.** A firm's risk arrives from two directions — from suppliers as input-cost uncertainty, from customers as output-price uncertainty — and the two are not symmetric: for a firm rich in growth and abandonment options, output-price uncertainty is partly good news while input-cost uncertainty is unambiguously bad.
  + 🧬 **Model.** Position in the production network determines the composition of the state vector priced by the firm's implied-volatility surface. The *origin* of uncertainty sets the sign of the spot–volatility correlation, the sign of the volatility risk premium, and the direction of the skew — but has no signed effect on the surface's level or curvature, which serves as a placebo.
  + ⏳ **Maturity separates the two.** Upstream uncertainty loads on short-dated volatility, downstream uncertainty on long-dated volatility, and a supply-chain partner's scheduled earnings announcement moves the firm's correlation in a predictable direction.

## 🎓 Teaching Innovation

- 🎲 [**Trading Games — live multiplayer classroom market simulations**](https://github.com/yingdongmao/trading-game) (FINC3014 *Trading and Dealing in Security Markets*, University of Sydney)
  + Five live multiplayer browser games hosted on a single **zero-dependency Python server**:
    - **Ticket Exchange** — no fundamental value; prices come from tastes. Call auction, then continuous trading (Week 1 limit vs. market orders).
    - **Open Cross** — private research intervals aggregate into one clearing price, then a continuous LOB (Week 2 auction market).
    - **Dealer Floor** — pure dealer market with persistent inventory, a Level-II ladder, and a plain-English "why you did / didn't trade" report (Week 2 dealer market).
    - **Dealer Pit LIVE** — continuous Glosten–Milgrom market where students *buy* early access to value, so the informed share is chosen by the room (Week 4 / Week 9 adverse selection and Kyle).
    - **Mystery Ticker** — trade against the house at a fixed spread while order flow drags the price to the hidden value (price-discovery demo).
  + Instructor switches modes from an admin console; students join from a **single URL by scanning a QR code**. Real-time projector charts: live supply/demand cross, LOB depth, dealer inventory drift, and the decay of |mid − V| against the clock — the slope *is* the speed of price discovery.
  + **Validated for 120 concurrent players, 0 errors, p95 latency ~25 ms** on a laptop.
  + Every player screen carries a "your move now" coach card and an order receipt, added after the first live runs so that students always know what their role requires and whether their last order did anything.

- 🗂️ [**A GitHub-native group assignment**](https://github.com/yingdongmao/finc3014-assignment-template) (FINC3014)
  + Students produce and submit the group project the way a quantitative research team does: one repository per group, stamped from a public **template repository** into a unit **organisation** owned by the teaching team.
  + Because the repos belong to the unit, groups cannot delete, rename, transfer, or accidentally expose their work, and repositories are protected at the deadline — the failure modes of student-created repos simply disappear.
  + Supporting tooling handles roster → repository creation, an acceptance dashboard, deadline protection, bulk collection, a **commit audit** that evidences each student's individual contribution, and generation of the per-group peer evaluation.
  + Built to replace **GitHub Classroom** after its retirement in August 2026, and documented so that a tutor who has never used Git can run the whole process.

### 📚 Skills
![Python](https://img.shields.io/badge/Python-3.8-blue) ![R](https://img.shields.io/badge/R-4.0.2-lightblue)
![LaTeX](https://img.shields.io/badge/LaTeX-Professional-orange)

🔗 [Google Scholar](https://scholar.google.com/citations?user=j0c2PTwAAAAJ&hl=en) | [Website](https://sites.google.com/view/yingdong-mao/home) | [LinkedIn](https://www.linkedin.com/in/yingdong-mao-022a45a1)
