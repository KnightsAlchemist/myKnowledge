The Random Forest classifier works by constructing an [[ensemble]] of [[decision trees]], each trained on a random subset of the data and [[features]] (using techniques like bagging and feature randomness). Each tree makes a prediction, and the final [[classification]] is determined by majority voting across all trees.

Core functioning:

1. **[[Data Bootstrapping]]**: Each tree is trained on a different subset of the data sampled with replacement (bootstrap aggregation or bagging), reducing variance.
2. **[[Feature Randomness]]**: During tree construction, only a random subset of features is considered for splitting at each node, improving model robustness and reducing correlation between trees.
3. **[[Voting]]**: Each tree independently predicts a class, and the Random Forest aggregates these predictions through majority voting for classification tasks (or averaging for regression).

This combination of randomness and ensemble learning makes Random Forest highly resistant to overfitting and capable of handling complex datasets with high-dimensional features.