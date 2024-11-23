
# Financial Model Predictions and Performance Analysis

This repository contains the results and performance metrics of financial prediction models applied across multiple datasets and configurations. The data is organized into different models experiments (`Bathla`, `Mohanty`, `Our Model`) and various assets or indices, such as `bp`, `cad-chf`, and `djia`. Each asset folder contains results for two preprocessing methodologies: `scale_split` and `split_scale`.

## Repository Structure

```
.
├── Bathla/
│   ├── bp/
│   │   ├── scale_split/
│   │   └── split_scale/
│   └── ...
├── Mohanty/
│   ├── bp/
│   │   ├── scale_split/
│   │   └── split_scale/
│   └── ...
└── Our Model/
    ├── bp/
    │   ├── scale_split/
    │   └── split_scale/
    └── ...
```

### Contents of Each Folder

Each `scale_split` and `split_scale` folder contains the following files:

1. **`final_predictions.csv`**  
   A CSV file detailing the predicted values, actual values, and the difference between them for the respective asset.

2. **`final_predictions.png`**  
   A line graph comparing the predicted and actual values, providing a visual representation of the model's performance.

3. **`final_training_metrics.png`**  
   A graph showing the model's training history, including metrics such as loss and accuracy over epochs.

4. **`performance_metrics.txt`**  
   A text file summarizing the model's performance metrics, such as:
   - Mean Absolute Error (MAE)
   - Mean Squared Error (MSE)
   - Root Mean Squared Error (RMSE)
   - Median Absolute Error (MdAE)
   - Mean Absolute Percentage Error (MAPE)

## Description of Methodologies

- **`scale_split`**: Preprocessing involves scaling the data first and then splitting it into training and testing sets.  
- **`split_scale`**: Preprocessing involves splitting the data first and then scaling each set separately.

These methodologies allow comparison of the effect of data scaling on model performance.

## Models and Assets

### Models
- **Bathla**: Experiment model replicated from *[Bathla, G. (2020)](https://ieeexplore.ieee.org/document/9315800)*, which investigates the application of LSTM networks for financial time series forecasting.
- **Mohanty**: Baseline model replicated from *[Mohanty, S. (2023)](https://www.ijfmr.com/research-paper.php?id=3345)*, focusing on traditional LSTM approaches for price prediction.
- **Our Model**: An enhanced predictive model built upon the findings of the aforementioned papers, leveraging advanced feature engineering and recurrent neural networks.


### Assets/Indices
Includes predictions and performance for the following:
- Stocks: `bp`, `dvn`, `ko`, `msft`
- Forex pairs: `cad-chf`, `eur-usd`, `usd-jpy`
- Indices: `djia`, `hsi`, `n225`

## Contact Information

For questions or further details, feel free to reach out via email:  
📧 **[research.parkera@outlook.com](mailto:research.parkera@outlook.com)**

---
