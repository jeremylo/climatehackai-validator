# Climate Hack.AI (2022) Submission Validator

This repository contains code that allows you to quickly validate your [Climate Hack.AI (2022)](https://climatehack.ai/) submission locally.

The files `features.npz` and `targets.npz` contain [EUMETSAT HRV Satellite Imagery](https://console.cloud.google.com/marketplace/product/bigquery-public-data/eumetsat-seviri-rss-hrv-uk) data preprocessed by Open Climate Fix and further processed into the format used for evaluation in [Climate Hack.AI 2022](https://climatehack.ai/), an international datathon between the student communities of 25 world-leading universities.

This validator uses 200 image sequences taken between 10am and 4pm over Great Britain from days sampled uniformly at random between January 2020 and November 2021 to score your submission.

## Instructions for use

0. Ensure you have NumPy, PyTorch and `pytorch_msssim` installed (as well as the other dependencies listed in the Climate Hack.AI getting started project).

1. Add the `validate.py` file to your existing submission folder, and the `features.npz` and `targets.npz` files one level up.

2. Change into the `submission/` directory (i.e. `cd submission`).

3. Run `validate.py` using Python 3.9 (e.g. `python validate.py`)

**Note**: this assumes the script specified in your `doxa.yaml` file is `evaluate.py` as by default, so you will need to modify `validate.py` if you have changed it.
