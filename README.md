# Audience Segmentation Analysis

Psychometric segmentation of consumer behavior data using clustering techniques.

This project demonstrates how to classify a population into meaningful audience groups based on values, attitudes, and behavioral patterns, going beyond simple demographic cuts. The approach produces actionable consumer profiles that can inform communication strategy, product positioning, and campaign personalization.

---

## The problem

Standard demographic segmentation (age, gender, income) tells you who your audience is, but not how they think or make decisions. Two consumers with identical demographics can have completely different values, motivations, and purchase behaviors.

Psychometric segmentation groups people by shared worldviews and behavioral patterns. The result is a typology that is more stable, more predictive, and more useful for strategic decisions than demographic cuts alone.

---

## What this project does

- Loads and explores a consumer opinion dataset with attitudinal and behavioral variables
- Scales psychometric variables for clustering
- Determines the optimal number of segments using the **Elbow Method** and **Silhouette Score**
- Applies **K-Means clustering** to classify respondents into segments
- Profiles each segment by attitudes, behaviors, and demographics
- Produces visualizations: radar chart, PCA map, segment size distribution

---

## Segments identified

| Segment | Label | Profile |
|---|---|---|
| 1 | Conscious Consumer | High sustainability engagement, willing to pay premium for ethical brands |
| 2 | Practical Consumer | Price and convenience driven, low brand loyalty |
| 3 | Aspirational Consumer | Brand and status oriented, influenced by trends and social proof |
| 4 | Traditional Consumer | Low digital engagement, conservative purchasing habits, high brand inertia |

---

## Project structure

```
audience-segmentation/
│
├── notebooks/
│   └── segmentation_walkthrough.ipynb   # Full analysis walkthrough
│
├── scripts/
│   └── segmentation.py                  # Reusable segmentation pipeline
│
└── README.md
```

---

## How to adapt to a new project

The script is built around a configurable list of psychometric variables and a target number of segments:

```python
PSYCHOMETRIC_VARS = [
    'your_attitude_variable_1',
    'your_attitude_variable_2',
    # ...
]

K = 4  # number of segments
```

Replace the variable list with your own attitudinal or behavioral columns and the pipeline runs end to end without further changes.

---

## Stack

- `Python 3.x`
- `Pandas` — data preparation and segment profiling
- `Scikit-learn` — K-Means clustering, StandardScaler, PCA, silhouette score
- `Matplotlib` — radar chart, PCA map, segment distribution
- `NumPy` — numerical operations

---

## Context

The methodology demonstrated here was applied in a national audience segmentation study (N = 4,256 probabilistic interviews) that produced a typology used to personalize communication campaigns across different population groups in Brazil. All data in this repository is synthetic and generated exclusively for demonstration purposes.

---

## Author

**Teresa De Bastiani**
Senior Market Research Analyst · Florianópolis, Brazil
[LinkedIn](https://linkedin.com/in/mteresadebastiani)
