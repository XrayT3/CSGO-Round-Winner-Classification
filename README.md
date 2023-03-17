# CSGO-Round-Winner-Classification
The model predicts which team will win using the state of each team.

Link to the dataset: https://www.openml.org/search?type=data&sort=runs&id=43430&status=active

# Data

Initially, I converted the dataset into .csv format and loaded it into a dataframe.
Having a dataframe first of all, I changed the main feature(round winner) from object to number format.
Then I got features with the most significant absolute correlation coefficient. In the end, I had data with 20 features.

# Model

Firstly, I tried the **K-NN algorithm** and got 75,97% accuracy. After searching hyperparameters, it increased to **77,76%**.
Not that much, but from that moment, I had the baseline.

Secondly, I tried the **random fores**t algorithm and got 82,32% accuracy. That's better. 
Then, I added more features with an absolute correlation coefficient more significant than 0.01. Using more features, the model achieved **88,01% accuracy**.
Trying to find better hyperparameters didn't give a better result.
