# Climate Hack.AI 2022 Submission Validator

This repository contains code to quickly verify your Climate Hack.AI (2022) submission locally!

The files `features.npz` and `targets.npz` contain 200 samples of [EUMETSAT HRV Satellite Imagery](https://console.cloud.google.com/marketplace/product/bigquery-public-data/eumetsat-seviri-rss-hrv-uk) data preprocessed by Open Climate Fix used in [Climate Hack.AI 2022](https://climatehack.ai/), an international datathon between the student communities of 25 world-leading universities. The data has been further processed into the same format used for evaluation in the competition.

## Instructions for use

0. Ensure you have NumPy, PyTorch and `pytorch_msssim` installed (as well as the other dependencies listed in the Climate Hack.AI getting started project).

1. Add the `validate.py` file to your existing submission folder, and the `features.npz` and `targets.npz` files one level up.

2. Change into the `submission/` directory (i.e. `cd submission`).

3. Run `validate.py` using Python 3.9 (e.g. `python validate.py`)
