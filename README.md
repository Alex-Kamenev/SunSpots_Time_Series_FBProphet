# Sunspot time-series forecasting

Course project exploring daily, monthly and yearly sunspot series with Prophet, stationarity tests and forecast cross-validation. The repository retains its historical name; Python imports use the maintained `prophet` package rather than `fbprophet` ([installation documentation](https://meta.github.io/prophet/docs/installation.html)).

Use Python 3.12 and run from this repository's root:

```text
python -m venv .venv
```

Activate the environment (`.venv\Scripts\Activate.ps1` in PowerShell), then:

```text
python -m pip install -r requirements.txt
python -m notebook Project_3.ipynb
```

`Project_3.ipynb` uses the included semicolon-delimited `data/daily.csv`, `data/monthly.csv` and `data/yearly.csv` datasets. `TS-Forecasting-FBProphet.ipynb` is an earlier example referencing `data/CR_timeSeries_Dataset.csv`, which is **not included**; supply that dataset before executing that example.

Yearly-series example forecasts use a yearly (`YS`) horizon. Stored notebook outputs are historical results and have not been recomputed after the package import and frequency updates. A small 60-row monthly fit and three-step prediction smoke test was run with Prophet 1.5.0; full forecast cross-validation was not rerun and can take considerable time. See the included assignment PDF for the original project brief.
