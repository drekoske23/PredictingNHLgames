NHL Game Outcome Prediction using Data Gathering Techniques, Feature Engineering, and Neural Networks

What is it?
This is a computer science project that uses data gathering techniques, feature engineering, and neural networks to create a neural network model that predicts the outcomes of NHL games being played today. The project consists of several Jupyter notebooks and CSV files that can be used to make predictions on NHL games. It is designed to be somewhat educational, highlighted by the inclusion of copious amounts of comments explaining the steps, but at its core, it is an effort to create the most successful model possible.

Accessing the Project
To access the project, follow these steps:

Clone this repository from Github: git clone https://github.com/drekoske23/PredictingNHLgames
Navigate to the project directory: cd repository
Run 'InteractiveModel.ipynb' to begin making predictions on today's NHL games.
However, all other .ipynb notebooks can be run by themselves without the need to follow the workflow of the project (i.e., cleaning, feature engineering, modeling), as the outputs of every notebook are included as a .csv, which is then read in by the next notebook.
The Notebooks and Their Purposes

Data Gathering/Cleaning Techniques
The data was downloaded from two different websites, both of which are linked in 'Cleaning.ipynb'. The pandas library was then used to assemble a cleaned dataframe that consisted of roughly 29,000 games, each of which had the score, date, and teams playing, represented by a 20-dimensional feature vector.

Feature Engineering
Two features were then created from the data to measure a team's recent performance: Elo and winstreak. Elo was a weighted measure of a team's performance that increased or decreased depending on the strength of the opponent team and the score of the game. The winstreak feature simply measures how many wins a team has in a row, quantifying its recent performance.

Model Training
The model was trained using a template neural network from tensorflow and keras. To create the best combination of hyperparameters, a grid search approach was used to test many combinations of hyperparameters and then select the best model based on minimizing the loss. That model is then saved so that the gridsearch function does not have to be rerun (it takes approximately 10 minutes to run).

Interactive Model
Finally, an interactive model was created. The notebook enables the user to read in the NHL games being played today and then performs the same feature engineering on this season's games. The last step involves reformatting the data so that it can be transformed into a tensor that is identical to the one the model was first trained on.

Conclusion
This project showcases how data gathering techniques, feature engineering, and neural networks can be used to predict the outcomes of NHL games. With its educational focus and comprehensive commenting, it is an excellent resource for those looking to learn more about these topics. By following the provided steps, users can easily access and utilize the project's Jupyter notebooks and CSV files to make predictions on NHL games being played today.
