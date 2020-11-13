# Gaming-Market-Exploration

### Business Objective: 

The main objective of this project is to explore and analyze the current video game market from both perspectives of developer and consumer.

1. For game developers, the question I would like to solve is what genre of games should they make, on which platform, via which publisher and etc, in order to achieve high profitability.

2. For consumers/gamers, the question I would like to solve is which game should they play next within their invested platforms based on the game content and their preference.

There are two datasets used in this project.

* The first dataset was obtained from https://www.kaggle.com/ashaheedq/video-games-sales-2019, it contains a list of video games with sales, critic and users score.

* The second dataset was scraped from https://www.vgchartz.com, it contains the hardware unit sales of current generation consoles.

#### Main notebook: https://github.com/dxljack/Gaming-Market-Exploration/blob/master/Gaming%20Market%20Analysis.ipynb

The project meets the following requirements:

1. Data Ingestion: 

- In part 1 of the notebook, I imputed missing values in the critic_score and global_sales columns by filling in with the average value of each genre, drop rows and columns with duplicated information, and etc.

- In part 4 of the notebook, I first scaped all possible game descriptions from IGDB then applied string processing on those descriptions. To be noted, the actuall scraping was done in a different notebook.

  * https://github.com/dxljack/Gaming-Market-Exploration/blob/master/Video%20game%20description%20scraping.ipynb

2. Visualization:

- Multiple plots are included in part 2 of the notebook, such as lineplot, barplot, piechart, and etc.

- Used tools including matplotlib, seaborn, and bokeh.

3. Machine Learning:

- In part 3 of the notebook, I first used linear regression to build a simple predictive model, further improved with ridge regression and eventually settled with randomforest regression with cross validation to obtain the best performing model to predict video game sales.

- In part 4 of the notebook, I first used string processing to tokenize game descriptions and build a simple recommendation system, further improved with nlp tool such as tf-idf to recommend video games.

4. Deliverable:

- Two Jupyter notebooks listed above.

- Interactive website is currently under testing, with working local serve. I will be adding interactive plots with bokeh before deployment.

  * https://github.com/dxljack/Game-Market-Webapp
