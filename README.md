# Predicting Relative Humidity using Long Short-Term Memory (LSTM)

This project aims to predict outdoor relative humidity (RH) in an Italian city using Long Short-Term Memory (LSTM), a powerful type of recurrent neural network (RNN) designed to handle sequence prediction tasks. 

**Relative humidity (RH)** is the amount of moisture in the air compared to the maximum amount of moisture the air can hold at a given temperature. It is a critical parameter influencing climate, agriculture, human health, and energy consumption. By leveraging LSTM, this study explores its capability to accurately forecast RH, contributing to fields such as weather forecasting, agriculture, and energy efficiency planning.

## Dataset and References
- **Dataset**: The dataset used for this study can be found at [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/360/air+quality).
- **Paper Reference**: For detailed methodology and findings, refer to [Outdoor Relative Humidity Prediction via Machine Learning Techniques](http://www.jeiletters.org/index.php?journal=mys&page=article&op=view&path%5B%5D=202100074).

## Motivation
In today's data-driven world, accurate prediction of RH is crucial for various applications including agriculture, health, and climate adaptation. LSTM, known for its ability to model sequential data effectively, offers a promising approach to capture the temporal dependencies in RH data.

## Methodology
This study focuses solely on the Long Short-Term Memory (LSTM) model due to its superior performance in time-series prediction tasks. LSTM is chosen for its capability to learn and remember patterns over long sequences, making it ideal for forecasting RH based on historical weather data.

By implementing LSTM, this project aims to advance the understanding and predictive capabilities of RH, facilitating better planning and decision-making in various sectors reliant on climate and environmental data.

---

## Dataset Information

The dataset comprises 9358 instances of hourly averaged responses recorded by 5 metal oxide chemical sensors in an Air Quality Chemical Multisensor Device. These sensors were deployed in a highly polluted urban environment at road level within an Italian city, spanning from March 2004 to February 2005. This dataset is the longest publicly available dataset from such sensors under real-world conditions.

### Features

| Variable Name | Role       | Type         | Description                                                            | Units          | Missing Values |
|---------------|------------|--------------|------------------------------------------------------------------------|-----------------|----------------|
| Date          | Feature    | Date         | Date                                                                   | -               | No             |
| Time          | Feature    | Categorical  | Time                                                                   | -               | No             |
| CO(GT)        | Feature    | Integer      | True hourly averaged concentration CO in mg/m^3 (reference analyzer)    | mg/m^3          | No             |
| PT08.S1(CO)   | Feature    | Categorical  | Hourly averaged sensor response (CO targeted)                           | -               | No             |
| NMHC(GT)      | Feature    | Integer      | True hourly averaged overall Non Metanic HydroCarbons concentration     | microg/m^3      | No             |
| C6H6(GT)      | Feature    | Continuous   | True hourly averaged Benzene concentration                               | microg/m^3      | No             |
| PT08.S2(NMHC) | Feature    | Categorical  | Hourly averaged sensor response (NMHC targeted)                         | -               | No             |
| NOx(GT)       | Feature    | Integer      | True hourly averaged NOx concentration                                   | ppb             | No             |
| PT08.S3(NOx)  | Feature    | Categorical  | Hourly averaged sensor response (NOx targeted)                           | -               | No             |
| NO2(GT)       | Feature    | Integer      | True hourly averaged NO2 concentration                                   | microg/m^3      | No             |
| PT08.S4(NO2)  | Feature    | Categorical  | Hourly averaged sensor response (NO2 targeted)                           | -               | No             |
| PT08.S5(O3)   | Feature    | Categorical  | Hourly averaged sensor response (O3 targeted)                            | -               | No             |
| T             | Feature    | Continuous   | Temperature                                                            | °C              | No             |
| RH            | Feature    | Continuous   | Relative Humidity                                                      | %               | No             |
| AH            | Feature    | Continuous   | Absolute Humidity                                                      | -               | No             |

This dataset includes evidence of sensor cross-sensitivities, concept drifts, and sensor drifts, which can affect concentration estimations. Missing values are denoted by -200.

**Note**: This dataset is exclusively intended for research purposes and is not licensed for commercial use.
