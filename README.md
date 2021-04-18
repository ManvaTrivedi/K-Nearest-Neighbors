# K-Nearest-Neighbors

Firstly, to create missingness in the dataset,for each feature I have removed 5%, 10% and 20% of values and marked them as missing.

I have performed 3 nearest neighbor imputation methods to find nearest neighbors:
(1)1-NN (2)k-NN (3)weighted k-NN
I have used Euclidean Distance and Manhattan Distance as distance measures.

Then as a result, I have calculated accuracy of imputation for each feature and stored it in "results.xlsx" file.

The output file lists the features and corresponding imputation accuracy for all possible combinations of methods, such as: 1-NN & Euclidean distance, 1-NN & Manhattan Distance, etc.

Now, while calculating the distance and training the model, if there is a significant difference in range, such as a a few ranging in the thousands versus a few ranging in the tens, it assumes that higher ranging numbers have some kind of supremacy. As a result, these larger numbers begin to play a larger role in the model's training.

So, I have implemented the above program using: (1)original data (2)applied Min-Max scaling (3)applied Standard scaling
