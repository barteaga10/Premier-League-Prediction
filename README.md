# English-Premier-League-Predictions
Bryan Arteaga 
## Overview 
The English premier league better know as epl is the worlds most competitive football league out there. With millions of spectators around the world we are starting to see in increase of wagers on results, scores, and championships. With money now bering on the line for football matches I would like to create a model that helps football fanatics, such as myself, and epl gamblers accurately predict the winner of said football matches to make smarter betting decisions using past results and betting odds. In order to create a model we used a data frame from kaggle and football co. These dataframe included details of roughly 6,000 previous premlier league matches from 2004 - 2020. The detail in these datasets included: home and away teams, the score, results, win or loss streak, betting odds, and many more. I merged both datasets, and analyzed over 3,000 games. I looked into each teams position on the table, their total points, streaks, and goal differential. Aftewards, I created a couple of predictive models, and chose the best one, a support vector classifier model. Which provided an accuracy score of 65%. Which means my model was able to predict if the home or away team won about 65% of the time.
## Business Problem
Create a model that helps football fanatics and epl gamblers accurately predict the winner of upcoming matches to make smarter betting decisions using past results and betting odds from previous seasons 
## Data Understanding 
I gathered my data from two different sources. The first source was from football co. Which contained results dating back to the 2003 and ending at 2021. This data contained details of roughly 6,500 matches. The details were home team, away team, the score, and results. And As well as the betting odds. My second source came from a kaggle dataset. It included 6,000 matches played from 2004 - 2018. The details included both the home and away goal differential throughout the season, and both teams standings and point on the table prior to the match. 
## Methods 
Since I had two datasets, I decided to merge both of them into one big dataframe. After doing so, I subset my features to mainly focus on details we knew prior to the upcoming match. Those features included: both team's goal differential, standings on the table, points, win/lose streak, and betting odds. Then proceeded to create a column that would indicate if the winning team was home or away or if the game ended in a draw.

After cleaning up my data, I continued to the next step, modeling. I ran a couple of models, but only one performed the best. The support vector model had the best results. The model used previous matches features to predict the winner. Preprocessing steps were done to prepare the features. This is included, creating a pipeline that one hot encode and scale my data.
## Results 
My best prediction socre came from a Support Vector Class. The model produced an accuracy score of 65%
## Conclusion
SVC Model was able to predict better than baseline models. Although, my model is struggling to predict draws, EPL Gamblers have better chance to accurately predict if the home or away team is going to win.
## Future Steps
Add more features for my model such as players for each team, Soccer Power Index, and injuries. Create a website that uses my model to predict the amount of profit each team would generate at the end of the season. And get my model to accurately predict if the match is going to end in a draw.
## Additional Sources
 * [Football Co](https://www.football-data.co.uk/englandm.php)
 * [Kaggle](https://www.kaggle.com/datasets/louischen7/football-results-and-betting-odds-data-of-epl?select=final_dataset_with_odds.csv)
 * [Presentation](Presentation.pdf)
 Repository Structure:
```
├── Notebooks                                  # code/project notebook
├── data                                       # data
├── Presentation.pdf                           # non-technical slides
├── EPL-Predictions.ipynb                      # code/project notebook
└── README.md                                  # the top-level README 
```