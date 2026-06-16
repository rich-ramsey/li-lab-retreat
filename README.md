# Data Science and Modelling Workshop

Materials for a workshop on tidy data, visualisation, and multilevel modelling in R, using simulated education research data.

## Authors 

Rich & Christian

## Workshop overview

The workshop covers three core ideas:

1. **FAIR data principles** — structuring your project so that sharing and reproducibility are defaults, not afterthoughts.
2. **Tidy data** — why long format matters, and how to get there with `tidyr`.
3. **Multilevel modelling** — why nested data structures call for varying effects, and how to fit them with `lme4`.

The exercises use simulated data from an embodied learning study in which participants
completed a knowledge test before and after a learning intervention (control vs. embodied condition).

## Repository structure

```
li-lab-retreat/
  exercises.qmd        # Main exercise document
  hints.qmd            # Hints organised by exercise — check here if you are stuck
  data_dictionary.md   # Variable descriptions for both datasets
  data/
    sim_data_simple_wide.csv   # Post-test data only, wide format
    sim_data_full_wide.csv     # Post-test and delay data, wide format
```

## Getting started

1. Open `li-lab-retreat.Rproj` in RStudio.
2. Install the required packages (see below).
3. Open `exercises.qmd` and work through the sections.
4. If you get stuck, open `hints.qmd` for some helpful tips.

## Required packages

```r
install.packages(c(
  "tidyverse",
  "lme4",
  "broom.mixed",
  "here"
))
```

## Data

Both datasets contain simulated data only.
No real participant data are included in this repository.
Data were simulated from a fitted model based on a real embodied learning study.

## License

This work is licensed under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).