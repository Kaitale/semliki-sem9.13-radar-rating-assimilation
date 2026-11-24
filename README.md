# Radar water-level observations for rating transfer, model diagnosis and forecast error correction in an operational flood forecasting system: the Semliki River, Uganda

**Kakooza, C. and Nafula, M. (2026).** KAI Water & Energy, Kampala, Uganda. Zenodo: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.24487523.svg)](https://doi.org/10.5281/zenodo.24487523)
Corresponding author: Monica Nafula, monicanafula@kaiwaterenergy.com

The paper transfers the dynamic rating of the Bweramule gauge (Kakooza et al., 2026, https://doi.org/10.5281/zenodo.24367492) 8.6 km upstream to the unrated REWC01 radar sensor, uses the hourly radar record to diagnose and recalibrate the fast response of the HEC-HMS model, and compares rainfall conditioning and error correction as forms of forecast updating in the HEC-HMS chain run under HEC-RTS.

## What is here

| File | Content |
|---|---|
| `Kakooza_et_al_2026_Semliki_radar_rating_forecast_updating.pdf` | the paper (12 pages, 5 figures, 6 tables) |
| `reproduce_paper.ipynb` | recomputes Tables 1–6 and the numbers of Sections 2 and 4 from the data; runs in seconds, locally or in [Google Colab](https://colab.research.google.com/github/Kaitale/semliki-sem9.13-radar-rating-assimilation/blob/main/reproduce_paper.ipynb) |
| `data_radar.zip` | ratings R2026-10 (Bweramule) and R2026-11 (radar); routed HEC-RAS steady profiles; hourly radar record on R2026-11 (8 Oct – 20 Nov 2026); HEC-HMS parameters above the radar; model flow components; catchment rain above the radar; structure tests; conditioned analyses and rain factors; correction-law scores; the 27-forecast test; the issue of 20 Nov 2026 |

## Run

```
pip install -r requirements.txt
jupyter notebook reproduce_paper.ipynb      # Run all
```

The notebook unzips `data_radar.zip` (or downloads it from this repository) and writes every table and figure to `outputs/`. The HEC-HMS runs themselves are not repeated (they need the model); their outputs at the radar junction are in the data.

## Data policy

The HEC-HMS and HEC-RAS models and the Bweramule gaugings are not distributed here; requests may be addressed to the corresponding author. Rainfall is from public products (CHIRPS, IMERG).

## Licence

Manuscript, data and figures: CC BY 4.0. Code and notebook code cells: MIT. See `LICENSE`.

## Cite

Kakooza, C., Nafula, M., 2026. Radar water-level observations for rating transfer, model diagnosis and forecast error correction in an operational flood forecasting system: the Semliki River, Uganda. Zenodo. https://doi.org/10.5281/zenodo.24487523
