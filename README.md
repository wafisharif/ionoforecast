# IonoForecast

An ML-ready ionospheric disturbance dataset and short-term forecasting system.

Built for NASA x Hack Club Stardance Challenge 2026.

## What this project does

The ionosphere — a charged layer of Earth's upper atmosphere — directly affects
GPS accuracy, radio communications, aviation, and power grids. When the Sun is
active, it disturbs the ionosphere and these systems degrade or fail.

This project:
1. Builds the first clean, unified, ML-ready dataset combining solar wind,
   geomagnetic indices, and ionospheric TEC measurements (1995–2024)
2. Trains a Temporal Fusion Transformer to forecast ionospheric disturbances
   1, 3, and 6 hours ahead with calibrated confidence intervals

## Data sources

| Source | Variables | Link |
|--------|-----------|------|
| NASA OMNI | Solar wind speed, density, Bz | omniweb.gsfc.nasa.gov |
| NOAA SWPC | Kp index, Dst index | swpc.noaa.gov |
| NASA/JPL GIM | Global ionospheric TEC maps | cddis.nasa.gov |
| NOAA NGDC | Flare/CME event labels | ngdc.noaa.gov |

## Project structure