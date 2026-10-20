# \# PEDAS 2026 — Machine Learning Classification

# 

# A machine learning classification project developed for \*\*PEDAS 2026\*\*, focusing on data preprocessing, feature engineering, and Random Forest classification.

# 

# \## Project Overview

# 

# This project builds a classification model to predict the category of each record based on the available dataset features. The workflow covers data preparation, feature engineering, model training, and prediction generation.

# 

# \## Methodology

# 

# The project follows these steps:

# 

# 1\. \*\*Data Loading\*\* — Load the labeled training dataset and unlabeled prediction dataset.

# 2\. \*\*Data Preprocessing\*\* — Prepare the data and normalize category labels.

# 3\. \*\*Feature Engineering\*\* — Extract features from domain information, URL characteristics, timestamps, and frequency-based information.

# 4\. \*\*Model Training\*\* — Train a Random Forest classifier using the labeled training data.

# 5\. \*\*Prediction\*\* — Generate category predictions for the unlabeled dataset.

# 

# \## Model

# 

# The final model uses `RandomForestClassifier` with the following configuration:

# 

# | Parameter | Value |

# |---|---|

# | `n\_estimators` | 100 |

# | `max\_depth` | `None` |

# | `min\_samples\_leaf` | 1 |

# | `max\_features` | `sqrt` |

# | `class\_weight` | `None` |

# | `random\_state` | 42 |

# 

# \## Repository Structure

# 

# ```text

# PEDAS-2026/

# ├── README.md

# ├── data/

# │   ├── training.csv

# │   └── predict.csv

# ├── notebooks/

# │   └── pedas2026\_final.ipynb

# └── submission/

# &#x20;   └── Tim Bebas-03.csv

# ```

# 

# \## Dataset

# 

# \- `training.csv` — Labeled data used to train the classification model.

# \- `predict.csv` — Unlabeled data used to generate predictions.

# 

# The dataset files are expected to be available in the `data/` directory.

# 

# \## Output

# 

# The prediction workflow produces category predictions for the records in `predict.csv`. The final submission file is provided separately in the `submission/` directory.

