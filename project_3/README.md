## Project 3: Subreddit Classifier

### Problem Statement
Going through Reddit posts can be addictive especially when interesting stories and posts comes in a row. However, wrongly classified posts from other subreddit can be such a web blanket when we are in the mood to continue reading. On top of which, when the number of wrongly classifed posts grow, it might just turn readers away. Therefore, it is important to tag our posts correctly for better reader experience. Therefore, building a model to suggest the correct label to writers will improve the chances of labeling posts correctly which will not only improve reader experience but also increase the browse rate of the posts which will indirectly motivate writers to post more often. The two chosen Subreddit for this analysis are Unresolved Mysteries and Cold Cases. The outcome success will be evaluated based on accuracy and the sensitivity of our model in classifying these two Subredits.

### Flow of This Analysis
Around 600 posts are scraped from each subreddit for this analysis. Features included are title, textbody and subreddit labels. This analysis will start with text cleaning using regular expression and different tokenization methods, followed by building the correct model to best predict subreddit labels. Lastly, we will take a look at our model performance by evaluating confusion matrix and various scores of our models. As an result, we decide our best model to be used in future subreddit classification.

### Contents:
1  Business Problem
2  Flow of This Analysis
3  Exploring Dataset
4  Data Cleaning
5  Modelling
6  Model Evaluation
7  Mis-Classification Analysis
8  Conclusion

### Conclusions and Recommendations
Recommendations:
All three models performs reasonably well on both train and unseen data. An accuracy score of 0.957 indicates that Random Forest Classifier is the clear winner for this task. It is capable of classifying almost all the posts. Having the lowest misclassification score of 0.043 also further proves that it is the best model of all the built ones.
This model can be used to
Classify subreddit posts which accidentally lost their labels
Move posts to the correct subreddit
Automatically suggest the correct subreddit label to writers to improve tagging accuracy
All of the above stated point will improve reader experience and increase the click through rate of writer's posts.

Limitations:
Unresolved Mystery being a much more popular subreddit than the cold cases provides us with more training text for our model to learn and improve its performance. Therefore, accuracy in predicting Unresolved Mystery will be better than that in predicting Cold Cases.
Nature and type of mysteries and cases are changing with time. Therefore, vocabulary features in this model needs to be constantly re-trained and updated to classify labels correctly.
Although this model performs reasonably well, we could try other classification methods such as Support Vector Machines. Furthermore, this model's performance is limited to two subreddit labels only and shall be tested with posts from more than two subreddits to evaluate its performance.