
## First Model: Approaches for dengAI submission

### 1. K-Polynomial Degree Algorithm

#### First submission: 
* We first established K-polynomial Degree approach baseline with Ridge regularization with no feature selection, lag 1-4 + rolling mean or city-specific grid alpha list. Only sin/cos seasonality approach for lower MAE results. This baseline ranking within the top 30%, results are shown table in belown.

| Best Score MAE | Current Rank      |
| -------------- | ----------------- |
| 27.1875        | 4491 out of 16812 |
* Now we add lag features approach using rolling_mean_4 (avg of 4 week), city-specific degree/alpha, and also feature selection (top-k) approach for better MAE result. Results are shown belown.


| Best Score MAE | Current Rank |
| -------------- | ------------ |
| 28.6442        | ....         |

### 2. Random Forest or XGBoost Algorithm





## Second Model: Predictions a couple weeks before