# TMDB Insights

# 

# Exploratory data analysis of the TMDB movies dataset, built as part of the Digital Futures data analytics training programme. The analysis looks at genre performance, the relationship between audience ratings and revenue, and a head-to-head franchise comparison between the Marvel Cinematic Universe and Pirates of the Caribbean.

# 

# Objective

# 

# Framed around a fictional recommendation platform ("Moviever"), the notebook investigates which patterns in the data are reliable signals of a film's commercial success and audience engagement, to inform what gets recommended to users.

# 

# What's in this repo

# moviever\_submission.ipynb — the full analysis notebook

# TMDB\_movies.csv — the dataset used

# Approach

# Cleaned and inspected the raw dataset: checked for missing values, parsed release dates for year-based grouping

# Exploded the nested genre and keyword fields (stored as JSON-like strings) to enable per-genre aggregation

# Compared genres by average revenue, profit, popularity, and film count

# Tested whether audience rating (vote\_average) predicts revenue

# Ran a matched-budget case study comparing Avengers: Age of Ultron against Pirates of the Caribbean: At World's End, then extended the comparison to franchise level (MCU vs. Pirates of the Caribbean as a whole)

# Key findings

# Genre: Action, Adventure, Animation, Family, Fantasy, and Science Fiction consistently outperform other genres on revenue, profit, and popularity. Action stands out as the strongest single recommendation, combining high performance with a large enough catalogue to serve recommendations repeatedly.

# Rating vs. revenue: revenue rises steadily as rating increases from 2 to 8, suggesting rating is a fairly reliable proxy for audience approval across most of the range. The drop-off at 9–10 reflects small sample sizes at the extremes rather than a genuine reversal.

# Matched-budget comparison: despite near-identical production costs, Age of Ultron significantly outgrossed At World's End with comparable audience ratings — pointing to franchise structure, not quality, as the deciding factor.

# Franchise level: the MCU generated roughly three times Pirates of the Caribbean's total franchise revenue. Its shared-universe model produces a consistently higher revenue floor than Pirates' catalogue ceiling, even at the level of individual films.

# Tools

# 

# Python, pandas, NumPy, Matplotlib, Seaborn

# 

# Running it

# 

# Clone the repo, then open moviever\_submission.ipynb in Jupyter (requires pandas, numpy, matplotlib, and seaborn). The notebook reads TMDB\_movies.csv from the same directory, so keep both files together.

