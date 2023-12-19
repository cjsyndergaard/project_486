# project_486
The purpose of this repository is to keep all of my project files. I've compiled what was useful in the project_clean.ipynb. 

The iteration and feedback process followed something similar to many projects. I began by looking at the data briefly, scaling it, threw some initial models at it, etc. Then I began to go down a path inspired by a project in STAT 666, where we were using cluster analysis in classification. I got feedback and assistance from friends in the MS program. I don't think this needs to be its own file, so I'm keeping it in the README.md.

I've also compiled why I believe I made a Tier 1 project with the other requirment types

Data: 
* My data had over 100,000 instances. I cleaned that down to just under 90,000.
* I standardized numeric, but it also had categorical variables.

Analysis:
* I did a LOT of feature engineering, particularly on the label feature. I would say that was the bulk of my project was exploring that since I know how machine learning methods work and didn't feel it was as necessary to explore that so much.
* I used random forests and naive bayes with minimal hyperparameter tuning.
* I used cluster analysis to look for strange observations, and I used it in an interesting way for feature engineering.
* I used UMAP as a dimension reduction technique (ended up not being super useful)
* I used SHAP to explore why my models were behaving as they did (rule of thumb - do NOT use SHAP when you have more than 50,000 instances, I had to use a sample of 100 to get mine to work in a reasonable (I stopped it originally at a 4 hour) time period).
* I was exploring a ML method called LVQ, which is like KNN except it seeks to speed up the prediction process by storing only several prototypes (like k means for classification, except it stores several centroids for the classes). I couldn't get it to work, so I found an alternative which was called nearest centroid, which stores the centroids of the groups and checks which centroid the new observation is closest to. 

Some of those didn't work as well as I hoped and others took a lot longer than expected, so I did 6 to make up for it instead of 5.

