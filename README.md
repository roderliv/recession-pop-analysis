# Recession Pop: Does Economic Hardship Make Music Happier?

Tests whether "recession pop," the idea that music gets more upbeat during economic downturns, is a real, measurable pattern. Combines decades of Spotify audio-feature data with U.S. unemployment and consumer sentiment data to look for a relationship, including lagged correlation and Granger causality analysis.

**[See the full analysis notebook](notebook.ipynb)**

## Setup

1. Clone this repo
2. Install dependencies: `pip install -r requirements.txt`
3. Get a free FRED API key at [fred.stlouisfed.org](https://fred.stlouisfed.org), and add it to a `.env` file: `FRED_API_KEY=your_key_here`
4. Download the Spotify dataset from [Kaggle](https://www.kaggle.com/datasets/yamaerenay/spotify-dataset-19212020-160k-tracks), create a `data/` folder in the project root if it doesn't already exist, and place the CSV files inside it
5. Run the notebook

## Key Findings

- Weak but statistically significant relationship between economic indicators and song valence (r ≈ 0.14)
- Effect is short-lived: Granger causality is only significant at 1-2 month lags
- Two independent indicators (unemployment, consumer sentiment) point the same direction, which adds credibility to a modest but real pattern
