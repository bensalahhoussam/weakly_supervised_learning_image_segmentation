# General concept 

The foundation of every machine learning project is data, the one thing you cannot do without.
The more data you get the more the model learns useful features ,increases performance and gets confident for better decisions ,but it can be a tedious job for data collection and annotation. 

To address this problem , there is a method called weakly semi-supervised learning or pseudo-labeling.

The main idea is to first train the model on labeled data , then use the trained model to predict on unlabeled data (Transfer learning method) , thus creating pseudo-labels,and will have more labeled data and continue doing that until the mode converges to higher performance.


