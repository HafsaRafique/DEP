# DIGITAL EMPOWERMENT PAKISTAN
This repository includes all tasks included in the internship program for a period of 4 weeks.

## WEEK 1: TIC-TAC-TOE GAME USING MINIMAX ALGORITHM
In a game of tic-tac-toe, the goal is to get 3 crosses/circles consecutively in a row/column or diagonally. Here, I have implemented a simple game using the minimax algorithm where the computer plays against the user.
### STEPS:
1.	The output of the game is displayed in a typical tic-tac-toe format and the program checks if a space has been filled beforehand.
   
2.	We specify the conditions required to win the game i.e: to get 3 crosses consecutively in a row/column/diagonally.
   
3.	We construct the minimax algorithm. X would be the mini player, trying to minimize the final score and O would be the max player, trying to maximize the final score. If max_checking is True, it is the player’s turn and if it is False, it’s the computer’s turn.
   
4.	When it’s the computer’s turn to play, it iterates all the places on the board where an O can be placed. It recursively calls the minimax function with max_checking set to True to simulate the player’s response.

5.	When it’s the player’s turn, it iterates all the places on the board where an X can be placed. It recursively calls the minimax function with max_checking set to False to simulate computer’s response.

6.	Based on this logic, the computer only makes the best move according to the best_score.

7.	If conditions are met by X, then player wins. If conditions are met by O, then computer wins. If the board space is filled, and no conditions are met then it’s a tie.

### RESULTS:
Below we see how the output looks like:

### SCENARIO 1:
<p align="center">
<image src="https://github.com/HafsaRafique/DEP/blob/main/images/Game_tied.png" width="500">
</p>

### SCENARIO 2:
<p align="center">
<image src="https://github.com/HafsaRafique/DEP/blob/main/images/Computer_won.png" width="300">
</p>


## WEEK 2: Implement a spam email classifier using machine learning algorithms like Naive Bayes or Support Vector Machines.

The following requirements were met:

1. Google Colab environment was used for this task.
   
2. The first step was to install all relevant libraries, to handle the dataset, to split the dataset and to plot the results.

3. The dataset was downloaded from Kaggle from the following link : [Spam email Dataset] (https://www.kaggle.com/datasets/jackksoncsie/spam-email-dataset)

4. The data was preprocessed and split into training and testing sets.

5. Vectorization was done to extract all important information from the text and create a numerical format for the data.

6. Support Vector Machine Algorithm was ultimately used for this task due to its exceptionally high accuracy for this task. SVM results showed 99.4% accuracy while Naive Bayes was only 95%.

7. The results were shown using classification report and a confusion matrix.

8. The classifier trained on the above dataset was then used to test out some sample email texts.


### RESULTS OF TRAINING:
The following shows the output of the trained classifier, the accuracy is shown to be around 99.4%:

<p align="center" style="border: 3 px">
<image src="https://github.com/HafsaRafique/DEP/blob/main/images/Classification_report.png" width="300">
</p>

The confusion matrix shows that the number of true positives and true negatives is significantly greater than false positives and negatives:

<p align="center" style="border: 3 px">
<image src="https://github.com/HafsaRafique/DEP/blob/main/images/Confusion_matrix.png" width="300">
</p>

### RESULTS OF TESTING:
A test was conducted using sample texts from emails to check the classifier's performance, the texts used were as follows:

1. Hi. We are thrilled to inform you that you've won the lottery. Contact 01234567 with 20$ to claim the prize!

2. Hi, Looking forward to seeing you at the party.

We see that the classifier correctly identified the texts:

<p align="center" style="border: 3 px">
<image src="https://github.com/HafsaRafique/DEP/blob/main/images/output.png">
</p>
   
