# Credit Card Customer Segmentation

## Overview
This notebook details the team’s clustering analysis to segment credit card customers into meaningful groups. The analysis provides insights to support targeted marketing, risk management, and customer engagement strategies.

## Key Steps
- Preprocessed and scaled features for clustering.
- Applied KMeans clustering and evaluated performance using **Silhouette Score** and **Davies–Bouldin Index**.
- Compared multiple k values to identify optimal cluster counts.

## Outcomes
- **k=3** provides broad customer categories: Revolvers, Low Activity, High-Frequency Transactors.
- **k=7** reveals granular subgroups including **VIP spenders**, **low-risk full payers**, and **dormant users**.
- Final recommendation: use **k=7** for detailed business actions, with **k=3** as a simplified view.
