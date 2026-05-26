# Awesome Macro Liquidity [![Awesome](https://awesome.re/badge.svg)](https://awesome.re) [![Lint](https://github.com/ruleaker/awesome-macro-liquidity/actions/workflows/lint.yml/badge.svg)](https://github.com/ruleaker/awesome-macro-liquidity/actions/workflows/lint.yml)

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
- [Podcasts](#podcasts)
- [Tools & Dashboards](#tools--dashboards)
- [Code & Templates](#code--templates)
- [Related](#related)

## Central Bank Data Sources

- [FRED](https://fred.stlouisfed.org/) - St. Louis Fed's database; free, comprehensive, has an API.
- [Federal Reserve H.4.1 Release](https://www.federalreserve.gov/releases/h41/) - Fed balance sheet, published weekly on Thursdays.
- [NY Fed System Open Market Account](https://www.newyorkfed.org/markets/desk-operations/soma) - Detailed holdings of the Fed's portfolio.
- [NY Fed Reverse Repo Operations](https://www.newyorkfed.org/markets/desk-operations/reverse-repo) - Overnight RRP volumes.
- [ECB Data Portal](https://data.ecb.europa.eu/) - European Central Bank data; replaces the older SDW.
- [Bank of Japan Statistics](https://www.boj.or.jp/en/statistics/) - Including Rinban operations and JGB holdings.
- [Bank of England Statistics](https://www.bankofengland.co.uk/statistics) - Monetary aggregates, balance sheet, gilt holdings.
- [PBOC Statistics](http://www.pbc.gov.cn/en/3688006/index.html) - People's Bank of China, English portal.
- [Swiss National Bank Data Portal](https://data.snb.ch/en) - FX reserves and balance sheet.
- [BIS Statistics](https://www.bis.org/statistics/index.htm) - Bank for International Settlements, cross-country aggregates.

## Key Liquidity Indicators

- [M2 Money Supply (M2SL)](https://fred.stlouisfed.org/series/M2SL) - Broadest US money stock measure.
- [Fed Balance Sheet (WALCL)](https://fred.stlouisfed.org/series/WALCL) - Total assets; weekly H.4.1 release.
- [Treasury General Account (WTREGEN)](https://fred.stlouisfed.org/series/WTREGEN) - Treasury cash that drains or adds bank reserves when issued or spent.
- [Overnight Reverse Repo (RRPONTSYD)](https://fred.stlouisfed.org/series/RRPONTSYD) - Cash parked at the Fed; rising RRP equals liquidity drain.
- [DXY Dollar Index](https://www.tradingview.com/symbols/TVC-DXY/) - Inverse proxy for global USD liquidity.
- [SOFR](https://fred.stlouisfed.org/series/SOFR) - Secured overnight rate; funding stress shows up here first.
- [Effective Fed Funds Rate (EFFR)](https://fred.stlouisfed.org/series/EFFR) - Daily-set policy rate proxy.
- [High-Yield Credit Spreads (BAML OAS)](https://fred.stlouisfed.org/series/BAMLH0A0HYM2) - Risk-on/off proxy via high-yield bond spreads.
- [TIPS 10-Year Breakeven](https://fred.stlouisfed.org/series/T10YIE) - Market-implied 10-year inflation expectations.
- [VIX Equity Volatility (VIXCLS)](https://fred.stlouisfed.org/series/VIXCLS) - The benchmark equity implied-vol index.
- [MOVE Index](https://www.tradingview.com/symbols/INDEX-MOVE/) - Treasury bond volatility; rates equivalent of VIX.

## Data Providers & APIs

- [FRED API](https://fred.stlouisfed.org/docs/api/fred/) - Official US macro data API; generous free tier.
- [TreasuryDirect](https://www.treasurydirect.gov/government/securities-research-tools/) - US Treasury issuance, auction results, TGA.
- [BIS Open Data](https://www.bis.org/statistics/data_index.htm) - Cross-country credit, debt, FX statistics.
- [IMF Data](https://www.imf.org/en/Data) - International balance of payments, reserves, IFS.
- [World Bank Open Data](https://data.worldbank.org/) - Long-run macro for ~200 countries.
- [OECD Data Portal](https://data.oecd.org/) - Developed-economies macro indicators.
- [TradingEconomics](https://tradingeconomics.com/) - Aggregator plus economic calendar; has an API.
- [Stooq](https://stooq.com/) - Free historical macro and equity data.
- [yfinance](https://github.com/ranaroussi/yfinance) - Yahoo Finance Python scraper.
- [Bloomberg Terminal](https://www.bloomberg.com/professional/products/bloomberg-terminal/) - Industry-standard institutional terminal. *(paid)*
- [Refinitiv Eikon](https://www.refinitiv.com/en/products/eikon-trading-software) - Bloomberg alternative. *(paid)*
- [Macrobond](https://www.macrobond.com/) - Macro time-series analytics. *(paid)*
- [Haver Analytics](https://www.haver.com/) - Macro data aggregator. *(paid)*

## Crypto-Native Liquidity

- [Glassnode](https://glassnode.com/) - On-chain BTC and ETH metrics; supply, flows, profitability.
- [CryptoQuant](https://cryptoquant.com/) - Exchange inflows/outflows, miner reserves, stablecoin flows.
- [Coinglass](https://www.coinglass.com/) - Derivatives data: funding rates, open interest, liquidations.
- [Velo Data](https://velodata.io/) - Institutional-grade derivatives and spot data.
- [DefiLlama](https://defillama.com/) - TVL across DeFi protocols, stablecoin supply, chain comparisons.
- [DefiLlama Stablecoins](https://defillama.com/stablecoins) - Stablecoin supply tracker; USDT and USDC growth as a crypto-native liquidity proxy.
- [Artemis](https://www.artemis.xyz/) - Cross-chain user, fee, and revenue analytics.
- [Dune Analytics](https://dune.com/) - Community SQL queries on Ethereum, Solana, and L2s.
- [Nansen](https://www.nansen.ai/) - Wallet labeling and smart-money flow tracking.
- [The Block Data](https://www.theblock.co/data) - Crypto market microstructure and exchange data.

## Research & Thinkers

- [Lyn Alden](https://www.lynalden.com/) - Newsletter blending macro, energy, and Bitcoin; rigorous and contrarian-friendly.
- [Arthur Hayes — Substack](https://cryptohayes.substack.com/) - Ex-BitMEX CEO; long-form macro essays linked to crypto positioning.
- [Raoul Pal — Real Vision](https://www.realvision.com/) - "Everything code", liquidity-cycle obsessive.
- [Mike Howell — CrossBorder Capital](https://www.crossbordercapital.com/) - Pioneered the Global Liquidity Index; foundational liquidity research.
- [Brent Johnson — Santiago Capital](https://www.santiagocapital.com/) - "Dollar Milkshake" thesis: USD strength drains global liquidity.
- [Hugh Hendry — Substack](https://hughhendry.substack.com/) - Ex-Eclectica; macro contrarian.
- [Cullen Roche — Pragmatic Capitalism](https://www.pragcap.com/) - Monetary plumbing, demystified.
- [Alf — The Macro Compass](https://themacrocompass.com/) - Central-bank focused, very accessible.
- [Russell Napier](https://www.solidground.online/) - Financial historian; long-cycle and great-reset frameworks.
- [Stanley Druckenmiller — Sohn Conference Talks](https://www.sohnconference.org/) - Speeches archive; concentrated liquidity-driven macro thinking.
- [Doomberg](https://doomberg.substack.com/) - Commodities and energy macro.
- [Bianco Research](https://www.biancoresearch.com/) - Rates and credit. *(paid)*

## Frameworks

- [Net Liquidity (Fed BS − TGA − RRP)](https://www.42macro.com/) - Most-cited liquidity proxy; popularized by 42 Macro.
- [Global Liquidity Index](https://en.wikipedia.org/wiki/Global_liquidity) - CrossBorder Capital's proprietary aggregate of cross-border liquidity flows.
- [Dollar Milkshake Theory](https://www.investopedia.com/dollar-milkshake-theory-7964570) - Brent Johnson; strong USD drains global liquidity into US assets.
- [Long-Term Debt Cycle](https://www.principles.com/the-changing-world-order/) - Ray Dalio; 50-75 year cycle of leverage build-up and deleveraging.
- [Minsky Moment](https://en.wikipedia.org/wiki/Minsky_moment) - Hyman Minsky; stability breeds instability, leverage cycles end in sudden deleveraging.
- [Reflexivity](https://en.wikipedia.org/wiki/Reflexivity_(social_theory)) - George Soros; market prices feed back into the fundamentals they are supposed to reflect.
- [Kondratiev Wave](https://en.wikipedia.org/wiki/Kondratiev_wave) - 50-year supercycle of innovation, credit expansion, and crisis.
- [All-Weather Portfolio](https://www.bridgewater.com/research-and-insights/the-all-weather-story) - Dalio; asset rotation across growth × inflation quadrants.

## Books

- [Howard Marks — Mastering the Market Cycle](https://www.goodreads.com/book/show/35840666-mastering-the-market-cycle) - Why and how to think about cycles.
- [Ray Dalio — Principles for Navigating Big Debt Crises](https://www.principles.com/big-debt-crises/) - Free PDF; archetype of debt-crisis playbook.
- [Lyn Alden — Broken Money](https://www.lynalden.com/broken-money/) - Monetary history through an energy-and-information lens.
- [Nassim Taleb — Antifragile](https://www.penguinrandomhouse.com/books/176227/antifragile-by-nassim-nicholas-taleb/) - Things that gain from disorder.
- [Nassim Taleb — The Black Swan](https://www.penguinrandomhouse.com/books/161741/the-black-swan-by-nassim-nicholas-taleb/) - The impact of the highly improbable.
- [George Soros — The Alchemy of Finance](https://www.wiley.com/en-us/The+Alchemy+of+Finance-p-9780471445494) - Reflexivity with diary case studies.
- [Benoit Mandelbrot — The Misbehavior of Markets](https://www.basicbooks.com/titles/benoit-b-mandelbrot/the-misbehavior-of-markets/9780465043576/) - Why returns are not Gaussian.
- [Michael Howell — Capital Wars](https://link.springer.com/book/10.1007/978-3-030-39288-8) - Global liquidity as the master variable.
- [Hyman Minsky — Stabilizing an Unstable Economy](https://www.mhprofessional.com/9780071592994-usa-stabilizing-an-unstable-economy) - Financial instability hypothesis source text.
- [Russell Napier — Anatomy of the Bear](https://www.harriman-house.com/anatomyofthebear) - Four great bear markets analyzed.
- [Walter Bagehot — Lombard Street](https://www.gutenberg.org/ebooks/4359) - 1873 central-banking foundational text; free Project Gutenberg edition.

## Podcasts

- [Odd Lots](https://www.bloomberg.com/oddlots) - Bloomberg's Joe Weisenthal and Tracy Alloway; technical macro deep dives.
- [Macro Voices](https://www.macrovoices.com/) - Erik Townsend; weekly expert interviews.
- [Forward Guidance](https://blockworks.co/podcast/forwardguidance) - Blockworks; Jack Farley; macro × crypto.
- [On The Margin](https://blockworks.co/podcast/on-the-margin) - Blockworks; Mike Ippolito; crypto-native macro.
- [The Compound and Friends](https://compoundinsight.com/) - Josh Brown and guests.
- [Macro Hive Conversations](https://macrohive.com/podcasts/) - Bilal Hafeez.

## Tools & Dashboards

- [TradingView Economies](https://www.tradingview.com/markets/economies-and-markets/) - Free macro charts and screens.
- [FRED Graph Builder](https://fredgraph.stlouisfed.org/) - Build custom multi-series charts, share by URL.
- [World Government Bonds](https://www.worldgovernmentbonds.com/) - Live sovereign yields and curves.
- [GuruFocus Economic Indicators](https://www.gurufocus.com/economic_indicators/) - Buffett indicator, Shiller PE, and more.
- [NY Fed Markets Data](https://www.newyorkfed.org/markets) - RRP, SOMA, primary dealer positions.
- [TIC Data (US Treasury)](https://home.treasury.gov/data/treasury-international-capital-tic-system) - Foreign holdings of US securities.
- [Checkonchain](https://charts.checkonchain.com/) - Free on-chain and macro composite dashboards.

## Code & Templates

- [fredapi](https://github.com/mortada/fredapi) - Python client for the FRED API.
- [pyfredapi](https://github.com/everett-sb/pyfredapi) - Modern alternative FRED client.
- [investpy](https://github.com/alvarobartt/investpy) - Investing.com scraper.
- [ccxt](https://github.com/ccxt/ccxt) - Unified crypto-exchange API for spot, perps, and funding.
- [Glassnode Studio API](https://docs.glassnode.com/) - On-chain metrics endpoint.
- [Dune SDK](https://dune.com/docs/api/) - Query Dune dashboards via API.

## Related

- [awesome-quant](https://github.com/wilsonfreitas/awesome-quant) - Quantitative finance ecosystem.
- [awesome-economics](https://github.com/iamericfletcher/awesome-economics) - Academic and applied economics.
- [awesome-defi](https://github.com/0xsequence/awesome-defi) - DeFi protocols and primitives.
- [awesome-blockchain](https://github.com/imbaniac/awesome-blockchain) - Blockchain landscape.

## Contributing

Contributions welcome. See [CONTRIBUTING.md](CONTRIBUTING.md) for the quality bar — actively maintained, primary source, substantively about liquidity, and a one-line description that tells the reader *why it matters*.
