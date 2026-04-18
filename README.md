Emotions in Music Analysis
Kaden Van Atta | Spring 2024
Tools: Python, Pandas, NumPy, Plotly
Dataset: 2,000 Spotify tracks across 10 genres

Overview
This project explores the emotional landscape of music by analyzing Spotify audio features across ten genres. Using valence, energy, tempo, danceability, acousticness, and instrumentalness as the core dimensions, the analysis maps how genre shapes emotional experience and identifies patterns that separate uplifting music from dark, intense, or melancholic tracks.

What's Inside
Valence vs. Energy Scatter Plot
The core emotional map of the dataset. Valence measures positivity and energy measures intensity, together forming four emotional quadrants: Happy/Excited, Content/Peaceful, Angry/Intense, and Sad/Dark. Each genre clusters visibly in this space.
Emotion Distribution by Genre
A stacked bar chart showing what percentage of each genre's tracks fall into each emotional zone. Reveals each genre's emotional personality at a glance.
Audio Feature Radar Chart
A spider chart overlaying all ten genres across five audio dimensions simultaneously, making it easy to see which features most differentiate genres from one another.
Danceability vs. Tempo
Examines the relationship between BPM and danceability with bubble size representing energy. Hip-Hop and R&B achieve high danceability at lower tempos while Metal runs fast but scores low on groove.
Acoustic vs. Instrumental Spectrum
Maps genres along two production axes with lowess trendlines. Classical sits at the acoustic and instrumental extreme while Electronic occupies the opposite end.
Genre Summary Table
Mean values for all audio features per genre, sorted by valence, presented in an interactive Plotly table.

Key Findings
Metal and Rock dominate the dark and intense emotional quadrant while Pop and Country skew toward happy and excited. Classical lands in the calm and peaceful zone, distinctly separated from every other genre by its low energy score of 0.27. Hip-Hop achieves the highest danceability in the dataset despite running at some of the lowest tempos, confirming that BPM alone does not drive groove. Genre proves to be a reliable proxy for emotional expectation, with each genre forming a distinct cluster in the valence-energy space.

How to Run

Clone the repo
Install dependencies: pip install pandas numpy plotly statsmodels
Open emotions_in_music_analysis.ipynb in Jupyter or Google Colab
If using Colab, upload spotify_data.csv to the session files panel
Run all cells

All charts render as interactive Plotly visualizations.
