# ARTI 308 – Lab 5: Feature Engineering for Classification

## Overview
This lab focuses on **feature engineering** for a classification task using a Talabat-style food delivery dataset. The goal is to predict `Order_Status` (Delivered, Cancelled, In Transit) using engineered features and a Random Forest classifier.

## Student Tasks

**Task 1 – New Engineered Feature**
Created `traffic_distance_interaction` by multiplying a numeric encoding of `Traffic_Level` (Low=1, Medium=2, High=3) by `Delivery_Distance_km`. This captures the combined delivery burden of congestion and distance in a single feature.

**Task 2 – Alternative Peak Hour Rule**
Tested a tighter peak window (12–14 and 20–22) vs. the original (12–15 and 19–23) and compared model accuracy to discuss sensitivity to the boundary definition.

**Task 3 – Comparing top_k Values**
Ran the model with `top_k = 10, 20, 30, 50` for `Item_Name_reduced` and compared accuracy and top feature importances across all four settings.

**Task 4 – Feature Selection**
Ran `SelectFromModel` with `threshold="median"` to keep only features above median importance, then compared accuracy with and without selection to evaluate whether it was beneficial.

