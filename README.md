# Spread of Congestion Analysis

## Overview

This repository contains analytical notebooks dedicated to understanding and visualizing the spread of traffic congestion using epidemiological models and data analysis techniques. Our approach draws parallels between the spread of diseases and the propagation of traffic congestion, employing the SIR (Susceptible - Infected - Recovered) model to analyze traffic data. This innovative methodology allows for a novel perspective on traffic analysis and congestion prediction.

## Contents

- `sir_modeling.ipynb`: Utilizes the SIR model to analyze and fit traffic data, drawing comparisons between disease spread and traffic congestion patterns.
- `sections_analysis.ipynb`: The core notebook for data processing, analyzing traffic congestion points, and visualizing them on maps. This notebook is essential for identifying critical congestion areas and understanding their distribution.
- `sys_meta_analysis.ipynb`: Computes aggregated results for various metrics, providing a comprehensive overview of the system's performance and the effectiveness of congestion mitigation strategies.

## Getting Started

To get started with the analysis, you will need to set up an environment capable of running Jupyter notebooks with Python. Ensure you have Python installed, along with the following major dependencies listed in the `requirements.txt` file.

It is recommended that the dependencies are installed through a virtual environment of your choice. Taking conda for example, you can create an environment for this repository using the following command:

```bash
conda create --name <env_name> --file requirements.txt
```

Alternatively, you can install these dependencies via pip:

```bash
pip install -r requirements.txt
```


After installing the necessary libraries, clone this repository and navigate into it:

```bash
git clone <repository-url>
cd Spread_of_Congestion
```

Once the repository is succesfully cloned, [navigate to the database storage and download the databases](https://drive.google.com/drive/folders/1gZ5YEo79munkY4b-V4b44c8qG3LJJuqv?usp=sharing). Move the databases (folders) into the `data` folder.

You can then start the Jupyter notebook server:

```bash
jupyter notebook
```

Navigate to the notebook of your choice in the browser interface that opens up.

### Dataset Overview

The `data` folder already includes the sections files that will define the scope of map for the experiments. 

The databases are folders whose naming format is `xxxxx_aa_bb_cc`, where `cc` indicates the percentage of stochastic route choice (SRC) users in each experiment. 

## Usage

- **SIR Modeling**: Open `sir_modeling.ipynb` to explore how the SIR model can be applied to traffic data. This notebook guides you through the process of fitting traffic congestion patterns to the SIR model, providing insights into the dynamics of congestion spread.
- **Sections Analysis**: Start with `sections_analysis.ipynb` for preprocessing and visual analysis of traffic data. This notebook focuses on identifying and visualizing congestion points, crucial for understanding congestion patterns.
- **System Meta Analysis**: For a holistic view of the congestion analysis, `sys_meta_analysis.ipynb` aggregates various metrics to evaluate overall system performance and the impact of different congestion mitigation strategies.

Note: You may need to edit the file paths at the top of each notebook to correctly import the data and export the results according to your local setup.

## Contributing

Contributions to this project are welcome. Please fork the repository, make your changes, and submit a pull request. For major changes, please open an issue first to discuss what you would like to change.

## License

[MIT License](LICENSE)
