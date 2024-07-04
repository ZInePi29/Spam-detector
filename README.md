## Spam Detector project

In this project I try to build a model that can tell if a message is spam or not.

**Steps:**
  1. The first step in this project was importing all the tools I was going to need. 
  2. Import the data, I did some manipulation on the DataFrame, such as, change the column names, map the label column to be 0s and 1s instead of 'ham' and 'spam'.
  3. Instantiate the model `MultinomialNB`.
  4. Split the data into X and y, then I used `TfidVectorizer` to transform the message (X) into a vector of numbers.
  5. Split the data into train and test sets, using `train_test_split` with `test_size=0.2` and fit the model to the train set.
  6. Score the model with the `score()` function. It returns the mean accuracy on the given test data.
  7. Check metrics with classification report and confusion matrix.
  8. Build a function that given a message, it transforms the message, then predict the label for the message and returns, in text, if it was 'Spam' or 'Ham'. 


