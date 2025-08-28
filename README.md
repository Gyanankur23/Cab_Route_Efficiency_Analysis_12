# Cab_Route_Efficiency_Analysis_12 CaseCraft Analytics Project Sprint Project 12

## 🚖 Overview  
This project evaluates cab route efficiency using synthetic geospatial and trip metadata. It blends clustering, regression modeling, and operational metrics to optimize urban mobility and fare calibration.

## 🎯 Objective  
To model cab trip efficiency using speed and fare-per-km, and predict route performance based on trip features.

## 📍 Dataset & Features  
- Trips: 1,000 synthetic cab rides  
- Features:  
  - Pickup & dropoff coordinates  
  - Duration (min), fare (₹), time of day  
  - Derived: distance (km), speed (km/h), fare per km  
- Target: `speed_kmph` (continuous)

## 📊 Visual Explorations  
- Histogram: Trip distance distribution  
- Histogram: Speed distribution  
- Scatterplot: Fare vs Distance (colored by time of day)  
- Clustering: K-Means on speed and fare/km  
- Scatterplot: Predicted vs Actual speed  
- Heatmap: Confusion matrix (binned speed)

## 🔍 Efficiency Clustering  
- 4 clusters based on speed and fare/km  
- Reveals distinct trip profiles: fast-cheap, slow-expensive, etc.  
- Evening trips show higher fare variability

## 🤖 Predictive Modeling  
- Model: Random Forest Regressor  
- Features: distance, duration, fare  
- Target: speed_kmph  
- Performance:  
  - Mean Absolute Error: **0.24 km/h**  
  - Confusion matrix confirms bin-level accuracy

## 🧠 Key Insights  
1. **Efficiency Drivers**: Speed and fare/km are key indicators  
2. **Temporal Impact**: Evening trips show more variability  
3. **Clustering Utility**: Identifies underperforming routes  
4. **Model Accuracy**: Low error in speed prediction  
5. **Operational Value**: Supports dispatch and fare calibration

## ✅ Final Conclusion  
Cab route efficiency can be effectively modeled using trip metadata and geospatial features. This framework enables predictive dispatching, fare optimization, and strategic identification of inefficient routes—ideal for urban mobility platforms.