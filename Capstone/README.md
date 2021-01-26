# Steam Game Recommender
*******

## Problem Statement

Steam is the largest game hosting platform, providing close to 90,000 games to players around the world. As an data scientist in Steam, my goal is to develop a personalized recommender system to recommend games to players base on their gaming preference. Evaluation of this project will be done via mean abosolute error(MAE) and average precision@5. 

This recommender system will eventually help Steam to:
1. Maintain player stickiness to the platform via tailored recommendations
2. Boost sales revenue through successfull recommendations to players

## Executive Summary

### Background
According to [study](https://www.mordorintelligence.com/industry-reports/global-games-market), global gaming market was valued at USD 162 billion in 2020 and is expected to reach a value of USD 295 billion by 2026. There is surge in both number of people playing video games and the types of video games produced by various developers to keep gamers engaged. 

The variety and count of games underpins the development of recommender systems which could suitably recommend games according to player's taste. Players will usually start a game or purchase a game if the recommendation list is short and tailored to his preference. However, recommendations made to the users are popularity based which means users are getting the same recommendations regardless of their preference. 

### Proposed Solution
Instead of using a popularity based system, more personalized model can be achieved using hybrid model consisting of both content based and collaborative filtering recommendations. We will be developing two models in this analysis:
- Collaborative filtering model (taking in user information and user ratings only)
- Hybrid model (taking in user information, user ratings and game descriptions)

These two models will try to predict user ratings for games available and recommend 5 games which are at top of the score board. In this way, this model is choosing the best set of games for each user. 

## Conclusions
Two models were built and tested in this project, collaborative filtering(CF) model and hybrid model. CF model has a MAE of 0.54 score and that for hybrid model is 0.64 score. The average precision@5 for CF model is around 37.49% and for hybrid model it is 60.82%. The higher precision of hybrid model indicates that incorporating game features such as game description will significantly boost model performance. Since, hybrid model has significantly better performance as compared to CF model, it is chosen as our production model. 

## Future Work
This model could be improved by including more input layers consisting of other game features such as owner count, average playtime etc to make predictions and recommendations more accurate.

In addition, we can consider time element in our future versions of recommender engine. Recent reviews and ratings should carry a higher weight as compared to older reviews and ratings. This is to capture user's change of preference and make our predictions more accurate.

Lastly, we want to find a way to speed up our recommender engine. The current recommender system could take couple of minutes before it can produce any recommendations. However, this is not acceptable in production environment, simply due to the fact that user would lost interest while waiting for our recommendations.

### Datasets Used
Complete [steam game dataset](https://www.kaggle.com/jesneuman/pc-games) and [user behavior dataset](https://www.kaggle.com/tamber/steam-video-gamess) from Kaggle are used in this project. There is total of 21,000 games and 12,000 users in this analysis. 