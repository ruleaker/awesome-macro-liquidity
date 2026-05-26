# Awesome Macro Liquidity [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of resources for tracking global macro liquidity — the underlying force that drives risk-asset cycles.

Liquidity moves everything before fundamentals catch up. This list collects the data sources, indicators, frameworks, thinkers, and tools that practitioners use to read it — across central banks, traditional markets, and on-chain.

Companion list: [awesome-derivatives-data](https://github.com/ruleaker/awesome-derivatives-data) — derivatives-side data (funding, OI, basis, options) that the macro flows feed into.

## Contents

- [Central Bank Data Sources](#central-bank-data-sources)
- [Key Liquidity Indicators](#key-liquidity-indicators)
- [Data Providers & APIs](#data-providers--apis)
- [Crypto-Native Liquidity](#crypto-native-liquidity)
- [Research & Thinkers](#research--thinkers)
- [Frameworks](#frameworks)
- [Books](#books)
- [Podcasts & Newsletters](#podcasts--newsletters)
- [Tools & Dashboards](#tools--dashboards)
- [Code & Templates](#code--templates)
- [Related Awesome Lists](#related-awesome-lists)
- [Contributing](#contributing)

## Central Bank Data Sources

- [FRED — Federal Reserve Economic Data](https://fred.stlouisfed.org/) — St. Louis Fed's database. Free, comprehensive, has an API.
- [Federal Reserve H.4.1 Release](https://www.federalreserve.gov/releases/h41/) — Fed balance sheet, published weekly (Thursdays).
- [NY Fed — System Open Market Account (SOMA)](https://www.newyorkfed.org/markets/desk-operations/soma) — Detailed holdings of Fed's portfolio.
- [NY Fed — Reverse Repo (RRP)](https://www.newyorkfed.org/markets/desk-operations/reverse-repo) — Overnight RRP volumes.
- [ECB Data Portal](https://data.ecb.europa.eu/) — European Central Bank data (replaces the older SDW).
- [Bank of Japan — Statistics](https://www.boj.or.jp/en/statistics/) — Including Rinban operations and JGB holdings.
- [Bank of England — Statistics](https://www.bankofengland.co.uk/statistics) — Monetary aggregates, balance sheet, gilt holdings.
- [PBOC — Statistics](http://www.pbc.gov.cn/en/3688006/index.html) — People's Bank of China, English portal.
- [Swiss National Bank — Data Portal](https://data.snb.ch/en) — FX reserves and balance sheet.
- [BIS Statistics](https://www.bis.org/statistics/index.htm) — Bank for International Settlements, cross-country aggregates.

## Key Liquidity Indicators

- **M2 (Broad Money, US)** — [M2SL on FRED](https://fred.stlouisfed.org/series/M2SL).
- **Fed Balance Sheet (Total Assets)** — [WALCL on FRED](https://fred.stlouisfed.org/series/WALCL).
- **Treasury General Account (TGA)** — [WTREGEN on FRED](https://fred.stlouisfed.org/series/WTREGEN). Treasury cash that drains/adds liquidity when issued/spent.
- **Reverse Repo (RRP)** — [RRPONTSYD on FRED](https://fred.stlouisfed.org/series/RRPONTSYD). Cash parked at Fed; rising RRP = liquidity drain.
- **Net Liquidity** — `Fed Balance Sheet − TGA − RRP`. The most-watched proxy among crypto/equity macro traders.
- **DXY (Dollar Index)** — [TVC:DXY](https://www.tradingview.com/symbols/TVC-DXY/). Inverse proxy for global USD liquidity.
- **SOFR** — [SOFR on FRED](https://fred.stlouisfed.org/series/SOFR). Secured overnight rate; funding stress shows up here first.
- **Effective Fed Funds Rate (EFFR)** — [EFFR on FRED](https://fred.stlouisfed.org/series/EFFR).
- **HY Credit Spreads (BAML HY OAS)** — [BAMLH0A0HYM2 on FRED](https://fred.stlouisfed.org/series/BAMLH0A0HYM2). Risk-on/off proxy.
- **TIPS 10Y Breakeven Inflation** — [T10YIE on FRED](https://fred.stlouisfed.org/series/T10YIE).
- **VIX** — [VIXCLS on FRED](https://fred.stlouisfed.org/series/VIXCLS). Equity vol.
- **MOVE Index** — Treasury bond vol; rates equivalent of VIX.

## Data Providers & APIs

- [FRED API](https://fred.stlouisfed.org/docs/api/fred/) — Official US macro data API; very generous free tier.
- [Treasury Direct](https://www.treasurydirect.gov/government/securities-research-tools/) — US Treasury issuance, auction results, TGA.
- [BIS Open Data](https://www.bis.org/statistics/data_index.htm) — Cross-country credit, debt, FX statistics.
- [IMF Data](https://www.imf.org/en/Data) — International balance of payments, reserves, IFS.
- [World Bank Open Data](https://data.worldbank.org/) — Long-run macro for ~200 countries.
- [OECD Data Portal](https://data.oecd.org/) — Developed economies macro.
- [TradingEconomics](https://tradingeconomics.com/) — Aggregator + economic calendar; has an API.
- [Stooq](https://stooq.com/) — Free historical macro & equity data.
- [yfinance (Python)](https://github.com/ranaroussi/yfinance) — Yahoo Finance scraper.
- *(Paid)* Bloomberg Terminal · Refinitiv Eikon · Macrobond · Haver Analytics.

## Crypto-Native Liquidity

- [Glassnode](https://glassnode.com/) — On-chain BTC/ETH metrics; supply, flows, profitability.
- [CryptoQuant](https://cryptoquant.com/) — Exchange inflows/outflows, miner reserves, stablecoin flows.
- [Coinglass](https://www.coinglass.com/) — Derivatives data: funding rates, open interest, liquidations.
- [Velo Data](https://velodata.io/) — Institutional-grade derivatives & spot data.
- [DefiLlama](https://defillama.com/) — TVL across DeFi protocols, stablecoin supply, chain comparisons.
- [DefiLlama Stablecoins](https://defillama.com/stablecoins) — Stablecoin supply tracker; USDT/USDC growth = crypto-native liquidity proxy.
- [Artemis](https://www.artemis.xyz/) — Cross-chain user, fee, and revenue analytics.
- [Dune Analytics](https://dune.com/) — Community SQL queries on Ethereum, Solana, L2s.
- [Nansen](https://www.nansen.ai/) — Wallet labeling, smart-money flow tracking.
- [The Block — Data](https://www.theblock.co/data) — Crypto market microstructure & exchange data.

## Research & Thinkers

- [Lyn Alden](https://www.lynalden.com/) — Newsletter blending macro, energy, and Bitcoin; rigorous and contrarian-friendly.
- [Arthur Hayes (Substack)](https://cryptohayes.substack.com/) — Ex-BitMEX CEO; long-form macro essays linked to crypto positioning.
- [Raoul Pal — Real Vision](https://www.realvision.com/) — Founder; "everything code", liquidity-cycle obsessive.
- [Mike Howell — CrossBorder Capital](https://www.crossbordercapital.com/) — Pioneered the Global Liquidity Index; foundational liquidity research.
- [Brent Johnson — Santiago Capital](https://www.santiagocapital.com/) — "Dollar Milkshake" thesis: USD strength drains global liquidity.
- [Hugh Hendry (Substack)](https://hughhendry.substack.com/) — Ex-Eclectica; macro contrarian.
- [Cullen Roche — Pragmatic Capitalism](https://www.pragcap.com/) — Monetary plumbing, demystified.
- [Alf — The Macro Compass](https://themacrocompass.substack.com/) — Central-bank focused, very accessible.
- [Russell Napier](https://www.solidground.online/) — Financial historian; long-cycle / great-reset frameworks.
- [Stanley Druckenmiller — Sohn Conference talks](https://www.sohnconference.org/) — Speeches archive; concentrated liquidity-driven macro thinking.

## Frameworks

- **Net Liquidity** — `Fed Balance Sheet − TGA − RRP`. Popularized by 42 Macro and used widely in crypto macro.
- **Global Liquidity Index (GLI)** — CrossBorder Capital's proprietary aggregate of cross-border liquidity flows.
- **Dollar Milkshake Theory** — Brent Johnson. A strong USD pulls global liquidity into US assets, starving the rest.
- **Long-Term Debt Cycle** — Ray Dalio. 50-75 year cycle of leverage build-up and deleveraging.
- **Minsky Moment** — Hyman Minsky. Stability breeds instability; leverage-driven cycles end in sudden deleveraging.
- **Reflexivity** — George Soros. Market prices feed back into the fundamentals they're supposed to reflect.
- **Kondratiev Wave** — ~50-year supercycle of innovation, credit expansion, and crisis.
- **All-Weather / 4 Quadrants** — Dalio. Asset rotation across growth × inflation environments.
- **Macro Compass Quadrants** — Alf. Real growth × monetary impulse, mapped to asset behavior.

## Books

- Howard Marks — *Mastering the Market Cycle* · *The Most Important Thing*
- Ray Dalio — *Principles for Navigating Big Debt Crises* · *Principles for Dealing with the Changing World Order*
- Lyn Alden — *Broken Money*
- Nassim Taleb — *Antifragile* · *The Black Swan* · *Fooled by Randomness* · *Dynamic Hedging*
- George Soros — *The Alchemy of Finance*
- Benoit Mandelbrot — *The Misbehavior of Markets*
- Michael Howell — *Capital Wars: The Rise of Global Liquidity*
- Hyman Minsky — *Stabilizing an Unstable Economy*
- Russell Napier — *Anatomy of the Bear* · *The Solid Ground*
- Felix Martin — *Money: The Unauthorized Biography*
- Walter Bagehot — *Lombard Street* (1873)

## Podcasts & Newsletters

**Podcasts**
- [Odd Lots](https://www.bloomberg.com/oddlots) — Bloomberg's Joe Weisenthal & Tracy Alloway; technical macro deep dives.
- [Macro Voices](https://www.macrovoices.com/) — Erik Townsend; weekly expert interviews.
- [Forward Guidance (Blockworks)](https://blockworks.co/podcast/forwardguidance) — Jack Farley; macro × crypto.
- [On The Margin (Blockworks)](https://blockworks.co/podcast/on-the-margin) — Mike Ippolito; crypto-native macro.
- [The Compound and Friends](https://compoundinsight.com/) — Josh Brown & guests.
- [Macro Hive Conversations](https://macrohive.com/podcasts/) — Bilal Hafeez.

**Newsletters**
- [Lyn Alden Research](https://www.lynalden.com/) — Free + paid premium.
- [The Macro Compass](https://themacrocompass.substack.com/) — Alf.
- [Arthur Hayes — Substack](https://cryptohayes.substack.com/) — Free.
- [Doomberg](https://doomberg.substack.com/) — Commodities & energy.
- [Bianco Research](https://www.biancoresearch.com/) — Rates & credit (paid).

## Tools & Dashboards

- [TradingView — Economies and Markets](https://www.tradingview.com/markets/economies-and-markets/) — Free macro charts and screens.
- [FRED Charting](https://fred.stlouisfed.org/) — Build custom multi-series charts, share by URL.
- [World Government Bonds](https://www.worldgovernmentbonds.com/) — Live sovereign yields and curves.
- [Trading Economics](https://tradingeconomics.com/) — Live economic calendar with consensus.
- [GuruFocus Economic Indicators](https://www.gurufocus.com/economic_indicators/) — Buffett indicator, Shiller PE, etc.
- [NY Fed Markets Data](https://www.newyorkfed.org/markets) — RRP, SOMA, primary dealer positions.
- [TIC Data (US Treasury)](https://home.treasury.gov/data/treasury-international-capital-tic-system) — Foreign holdings of US securities.

## Code & Templates

- [`fredapi` (Python)](https://github.com/mortada/fredapi) — Query FRED programmatically.
- [`pyfredapi`](https://github.com/everett-sb/pyfredapi) — Modern alternative FRED client.
- [`investpy`](https://github.com/alvarobartt/investpy) — Investing.com scraper.
- [`yfinance`](https://github.com/ranaroussi/yfinance) — Yahoo Finance.
- [`ccxt`](https://github.com/ccxt/ccxt) — Unified crypto exchange API; spot + perps + funding.
- [Glassnode Studio API](https://docs.glassnode.com/) — On-chain metrics endpoint.
- [Dune SDK](https://dune.com/docs/api/) — Query Dune dashboards via API.

## Related Awesome Lists

- [awesome-derivatives-data](https://github.com/ruleaker/awesome-derivatives-data) — Sister list; derivatives-side data (funding, OI, basis, options, microstructure).
- [awesome-quant](https://github.com/wilsonfreitas/awesome-quant) — Quantitative finance ecosystem.
- [awesome-economics](https://github.com/iamericfletcher/awesome-economics) — Academic & applied economics.
- [awesome-defi](https://github.com/0xsequence/awesome-defi) — DeFi protocols and primitives.
- [awesome-blockchain](https://github.com/imbaniac/awesome-blockchain) — Blockchain landscape.

## Contributing

Contributions welcome. See [CONTRIBUTING.md](CONTRIBUTING.md). Open a PR with new resources that meet the bar:

- Actively maintained and accessible
- Substantively about **liquidity** (not generic macro/finance commentary)
- One-line description that tells the reader *why it matters*

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the curator has waived all copyright and related or neighboring rights to this work.
