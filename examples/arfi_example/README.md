# Simulation study

*This project was rendered with ASReview-Makita version 0.1.1+88.g0103c56.dirty.*

This project was rendered from the Makita-ARFI template. See [asreview/asreview-makita#templates](https://github.com/asreview/asreview-makita#templates) for template rules and formats.

The template is described as: 'All Relevant, Fixed Irrelevant'.

## Installation

This project depends on Python 3.7 or later (python.org/download), and [ASReview](https://asreview.nl/download/). Install the following dependencies to run the simulation and analysis in this project.

```sh
pip install asreview asreview-insights asreview-datatools
```

## Data

The performance on the following datasets is evaluated:

- data/ptsd_again.csv
- data/ptsd.csv

## Run simulation

To start the simulation, run the following command in the project directory.

```sh
sh jobs.sh
```

## structure

The following files are found in this project:

    📦
    ├── 📂data
    │   ├── 📜ptsd_again.csv
    │   ├── 📜ptsd.csv
    ├── 📂output
    │   ├── 📂simulation
    |   |   └── 📂ptsd_again
    |   |       ├── 📂descriptives
    |   |       |   ├── 📜data_stats_ptsd_again.json
    |   |       |   ├── 📜wordcloud_ptsd_again.png
    |   |       |   ├── 📜wordcloud_relevant_ptsd_again.png
    |   |       |   └── 📜wordcloud_irrelevant_ptsd_again.png
    |   |       ├── 📂state_files
    |   |       |   ├── 📜sim_ptsd_again_`x`.asreview
    |   |       |   └── 📜...
    |   |       ├── 📜metrics_sim_ptsd_again_`x`.json
    |   |       ├── 📜...
    |   |       └── 📜plot_recall_ptsd_again.png
    |   |   └── 📂ptsd
    |   |       ├── 📂descriptives
    |   |       |   ├── 📜data_stats_ptsd.json
    |   |       |   ├── 📜wordcloud_ptsd.png
    |   |       |   ├── 📜wordcloud_relevant_ptsd.png
    |   |       |   └── 📜wordcloud_irrelevant_ptsd.png
    |   |       ├── 📂state_files
    |   |       |   ├── 📜sim_ptsd_`x`.asreview
    |   |       |   └── 📜...
    |   |       ├── 📜metrics_sim_ptsd_`x`.json
    |   |       ├── 📜...
    |   |       └── 📜plot_recall_ptsd.png
    │   └── 📂tables
    |       ├── 📜data_descriptives.csv
    |       ├── 📜data_descriptives.xlsx
    |       ├── 📜data_metrics.csv
    |       └── 📜data_metrics.xlsx
    ├── 📂scripts
    │   ├── 📜get_plot.py
    │   ├── 📜merge_descriptives.py
    │   ├── 📜merge_metrics.py
    │   └── 📜...
    ├── 📜jobs.sh
    └── 📜README.md
