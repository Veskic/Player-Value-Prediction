# 🎮 Player Market Value Prediction (FIFA 21)

This project uses machine learning to predict the market value of football players using their physical and technical attributes, based on the FIFA 21 dataset.

## 📂 Project Structure

```bash
Player-Value-Prediction/
│
├── 01_data_cleaning.ipynb         # Load and clean raw data
├── 02_model_training.ipynb        # Train RandomForestRegressor on cleaned data
├── 03_unlisted_prediction.ipynb   # Predict values for unlisted (0 value) players
├── 04_undervalued_players.ipynb   # Detect undervalued players by comparing predicted vs actual
├── 05_predict_value.ipynb         # Interactive prediction
│
├── Data/
│   └── players_21.csv             # Original dataset
│
├── Results/
│   ├── predicted_unlisted.csv
│   └── undervalued_players.csv
│
├── figures/
│   ├── feature_importance_chart.png
│   ├── top10_unlisted.png
│   └── top10_undervalued_chart.png
│
├── model/
│   └── fifa_value_model.pkl       # Trained model
│
│
├── requirements.txt
└── README.md
```
## 📊 Dataset

- **Source:** [Kaggle - FIFA 21 Complete Player Dataset](https://www.kaggle.com/datasets/stefanoleone992/fifa-21-complete-player-dataset)
- **Rows:** ~18,944 total players
- **After Cleaning:** ~16,654 players
- **Target Variable:** `value_eur` (market value in Euros)

---

## 🛠️ Technologies

- Python (3.10+)
- Libraries: Pandas, NumPy, scikit-learn, Matplotlib
- Jupyter Notebooks

---

## 💡 Features

- Predict market value of players without official value
- Detect undervalued players by comparing predicted vs actual
- Visualize feature importances and top predictions
- Input new player stats and get instant value prediction
- Export results to CSV for further analysis
