# XAGUSD 5m OHLCV Metals Historical Data — Free Sample

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE) [![Dataset rows](https://img.shields.io/badge/full_dataset-1_197_314_rows-blue)](https://ork.ad/) [![Updated](https://img.shields.io/badge/weekly_update-every_Sunday-green)](https://ork.ad/) [![Full data on ork.ad](https://img.shields.io/badge/download-ork.ad-orange)](https://ork.ad/)

### → [**Download the full XAGUSD dataset on ork.ad**](https://ork.ad/)

**XAGUSD 5m OHLCV Precious metals historical data** — ultra high-quality 5m OHLCV for **Silver / US Dollar**. Near-continuous precious-metals liquidity across global sessions. Clean `time, open, high, low, close, volume` CSV for backtesting, algorithmic trading and quantitative research.

## Table of contents

- [Why this dataset?](#why-this-dataset)
- [Download sample CSV](#download-sample)
- [GitHub Pages preview](#github-pages)
- [Sample vs full dataset](#sample-vs-full-dataset)
- [Timeframes on ork.ad](#timeframes-on-orkad)
- [Weekly updates](#weekly-updates)
- [Data preview](#data-preview)
- [Schema](#schema)
- [Code examples](#code-examples)
- [Download full data on ork.ad](#download-full-data)

## Why this dataset?

- **Ultra high-quality 5m OHLCV** for **Silver / US Dollar** (Precious metals)
- **Near-continuous precious-metals liquidity across global sessions**
- **Clean CSV schema** — `time, open, high, low, close, volume` (no gaps in formatting)
- **Free evaluation sample** on GitHub (`5m`) · **13 timeframes** on [ork.ad](https://ork.ad/) · **1,197,314** `5m` rows in the full archive
- Built for **backtesting**, **algorithmic trading** and **quantitative finance** workflows
- **Weekly refresh** — [ork.ad](https://ork.ad/) every **Sunday**; GitHub `5m` sample updated in sync

> **Sample on GitHub** · `XAGUSD_5m.csv` (35,508 rows, `2026-01-04` → `2026-07-03`). **Full archive on [ork.ad](https://ork.ad/)** — **1,197,314** `5m` rows (~59.15 MB), **13 timeframes** (``1m`, `3m`, `5m`, `15m`, `30m`, `1H`, `2H`, `4H`, `8H`, `12H`, `16H`, `1D`, `1W``), `2009-02-24` → `2026-07-03`.

## Download sample

**[XAGUSD_5m.csv](https://github.com/ork-ad/xagusd-5m-ohlcv-metals-historical-data/blob/main/XAGUSD_5m.csv)** on GitHub ([raw CSV](https://raw.githubusercontent.com/ork-ad/xagusd-5m-ohlcv-metals-historical-data/main/XAGUSD_5m.csv)) · [GitHub Releases](https://github.com/ork-ad/xagusd-5m-ohlcv-metals-historical-data/releases) when the release workflow is active.

## GitHub Pages

Interactive chart & stats: **[https://ork-ad.github.io/xagusd-5m-ohlcv-metals-historical-data/](https://ork-ad.github.io/xagusd-5m-ohlcv-metals-historical-data/)**

## Sample vs full dataset

| | **Sample (this repo)** | **Full dataset ([ork.ad](https://ork.ad/))** |
|---|--:|---|
| Instrument | Silver / US Dollar · Precious metals | Silver / US Dollar · Precious metals |
| Timeframes | `5m` (sample) | **13** — `1m`, `3m`, `5m`, `15m`, `30m`, `1H`, `2H`, `4H`, `8H`, `12H`, `16H`, `1D`, `1W` |
| 5m rows | 35,508 | **1,197,314** |
| Size | 1.8 MB | ~59.15 MB |
| Period | `2026-01-04` → `2026-07-03` | `2009-02-24` → `2026-07-03` |
| File | `XAGUSD_5m.csv` | ZIP on [ork.ad](https://ork.ad/) |
| Updates | Weekly (Sunday) — GitHub sample | Weekly (Sunday) — all timeframes |

## Timeframes on ork.ad

This GitHub repository ships a **`5m` evaluation sample** only. On **[ork.ad](https://ork.ad/)**, each full asset archive is delivered as a ZIP with **13 gap-free OHLCV timeframes** (one CSV per timeframe):

**1m** · **3m** · **5m** · **15m** · **30m** · **1H** · **2H** · **4H** · **8H** · **12H** · **16H** · **1D** · **1W**

GitHub = `5m` sample · [ork.ad](https://ork.ad/) = all **13** timeframes above for the same instrument.

## Weekly updates

- **[ork.ad](https://ork.ad/)** — Full datasets on ork.ad are updated every Sunday.
- **GitHub (this repo)** — GitHub samples are refreshed weekly (every Sunday), in sync with ork.ad.

When a new `5m` sample is published on GitHub, the README, chart preview and CSV reflect the latest week of data.

## Data preview

First and latest rows from the GitHub sample **`XAGUSD_5m.csv`**:

**First rows**

| time | open | high | low | close | volume |
| --- | --- | --- | --- | --- | --- |
| 2026-01-04T23:00:00Z | 72.503 | 73.449 | 72.503 | 73.233 | 2944 |
| 2026-01-04T23:05:00Z | 73.233 | 73.243 | 72.836 | 73.071 | 3301 |
| 2026-01-04T23:10:00Z | 73.071 | 73.324 | 73.025 | 73.295 | 2117 |
| 2026-01-04T23:15:00Z | 73.295 | 73.345 | 73.006 | 73.094 | 2303 |
| 2026-01-04T23:20:00Z | 73.094 | 73.199 | 73.034 | 73.045 | 1492 |

**Last rows**

| time | open | high | low | close | volume |
| --- | --- | --- | --- | --- | --- |
| time | open | high | low | close | volume |
| 2026-07-03T20:20:00Z | 62.171 | 62.298 | 62.147 | 62.187 | 7 |
| 2026-07-03T20:25:00Z | 62.187 | 62.187 | 62.181 | 62.184 | 3 |
| 2026-07-03T20:30:00Z | 62.184 | 62.2 | 62.164 | 62.2 | 8 |
| 2026-07-03T20:35:00Z | 62.2 | 62.2 | 62.194 | 62.194 | 3 |

## Schema

```text
time,open,high,low,close,volume
```

## Code examples

### pandas

```python
import pandas as pd

df = pd.read_csv('XAGUSD_5m.csv', parse_dates=['time'])
df.set_index('time', inplace=True)
print(df.describe())
print(df.resample('1h').agg({'open': 'first', 'high': 'max',
                              'low': 'min', 'close': 'last', 'volume': 'sum'}).head())
```

### backtrader

```python
import backtrader as bt
import pandas as pd

df = pd.read_csv('XAGUSD_5m.csv', parse_dates=['time'])
df.set_index('time', inplace=True)

class PandasData(bt.feeds.PandasData):
    params = (('datetime', None), ('open', 'open'), ('high', 'high'),
              ('low', 'low'), ('close', 'close'), ('volume', 'volume'))

cerebro = bt.Cerebro()
cerebro.adddata(PandasData(dataname=df))
# cerebro.addstrategy(YourStrategy)
# cerebro.run()
```

### vectorbt

```python
import pandas as pd
import vectorbt as vbt

df = pd.read_csv('XAGUSD_5m.csv', parse_dates=['time'])
close = df.set_index('time')['close']
fast, slow = vbt.MA.run(close, 10), vbt.MA.run(close, 50)
entries = fast.ma_crossed_above(slow)
exits = fast.ma_crossed_below(slow)
pf = vbt.Portfolio.from_signals(close, entries, exits, init_cash=10_000, freq='5min')
print(pf.stats())
```

## Download full data

The complete **XAGUSD** archive on **[ork.ad](https://ork.ad/)** includes **13 OHLCV timeframes** (`1m`, `3m`, `5m`, `15m`, `30m`, `1H`, `2H`, `4H`, `8H`, `12H`, `16H`, `1D`, `1W`) — **1,197,314** rows at `5m`, plus all other timeframes in the same ZIP.

**[→ Get the full XAGUSD dataset on ork.ad](https://ork.ad/)**

---
*GetData · XAGUSD 5m OHLCV sample on GitHub · Full historical data on [ork.ad](https://ork.ad/) · 2026-07-06 UTC*