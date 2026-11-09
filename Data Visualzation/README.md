# Human vs AI Essays - Data Visualization (Task 3)

**Question:** Do human-written essays and AI-written essays look different?

## Dataset
DAIGT "LLM - Detect AI Generated Text" essays (`train_v2_drcat_02.csv`), originally from Kaggle. A random sample of 6,000 essays (random_state=42) is saved as `human_vs_ai_essays_sample.csv`. After removing duplicates, about 60% are human and 40% are AI.

## Libraries
pandas, numpy, matplotlib, seaborn, scikit-learn (only for the stopword list)

Install: `pip install -r requirements.txt`

## Files
- `task3_data_visualization.ipynb` - the full analysis with Matplotlib and Seaborn charts
- `human_vs_ai_dashboard.html` - interactive dashboard and data story (open in any browser)
- `human_vs_ai_essays_sample.csv` - the 6,000-essay sample used
- `images/` - all charts as PNG files
- `requirements.txt` - libraries to install

## Charts (saved in `images/`)
1. Pie chart - human vs AI share
2. Histogram - essay length in words
3. Box plot - average word length
4. Violin plot - unique-word ratio
5. Scatter plot - word count vs unique-word ratio
6. Heatmap - correlation of text features
7. Bar charts - top 10 words for each group
8. Bar charts - commas and sentence length
9. Dashboard - 4 charts summarizing the findings

## Key insights
- Human essays are longer (about 419 words vs 330) and have longer sentences.
- AI essays use more commas and slightly longer words.
- The groups overlap a lot, so no single feature is enough to detect AI text.

## How to run
Open `task3_data_visualization.ipynb` in Jupyter, keep the CSV in the same folder, and run all cells.

## License
The code, notebook, charts and dashboard are released under the MIT License (see `LICENSE`).
The essay data comes from the DAIGT dataset on Kaggle and is **not** covered by this license. Check the original dataset's terms before reusing or redistributing it.
