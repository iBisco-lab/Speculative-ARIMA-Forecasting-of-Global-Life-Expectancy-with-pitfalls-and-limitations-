# Speculative ARIMA Forecasting of Global Life Expectancy (with pitfalls and limitations)

## Disclaimer (read this first)
This project is a **purely speculative analysis**.  
It explores *whether* and *how* an **ARIMA** time-series model could be applied to historical **global life expectancy** data, and it intentionally highlights the **problematic aspects** of doing so.

This is **not** a scientific forecast, not a causal model, and not a reliable basis for policy/medical conclusions.

## What this project tries to do
- Use historical global life expectancy estimates (1950–2019) to fit an ARIMA model and produce a forward projection.
- Compare short-horizon predictions against held-out values to gauge rough fit.
- Discuss why “a forecast that keeps going up” does **not** answer questions like “Is there a limit to human lifespan?”

The accompanying write-up explicitly separates **life expectancy** from **maximum lifespan** and notes that increasing life expectancy does not imply the disappearance of a lifespan bound. (See `docs/`.)  

## Data
- Source: UN World Population Prospects (2022 Revision) life expectancy estimates are referenced in the report.
- The report mentions the removal of 2020–2021 values due to the pandemic shock, because a plain ARIMA model is not designed to handle such structural breaks.
