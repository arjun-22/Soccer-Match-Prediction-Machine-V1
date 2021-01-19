# Soccer-Match-Prediction-Model-V1

I created a machine learning model to predict the outcomes for Manchester United home matches. To predict the outcome for each game, I used the data from 149 Manchester United home games from 2008-2016 to train a multinomial logistic regression classifier.

The features for the classifier were: 
 1. Manchester United formation
 2. Manchester United goalkeeper rating
 3. Manchester United defense rating
 4. Manchester United midfield rating
 5. Manchester United offense rating
 6. Away team formation
 7. Away team goalkeeper rating
 8. Away team defense rating
 9. Away team midfield rating
 10. Away team offense rating
 
The goalkeeper rating for each team was the rating for the goalkeeper from the videogame FIFA. The defense rating for each team was the average of the ratings for each of the defenders of each team from FIFA. The midfield rating for each team was the average of the ratings for each of the midfielders of each team from FIFA. The offense rating for each team was the average of the ratings for each of the attackers of each team from FIFA. For example, if Manchester United’s lineup consisted of four defenders whose ratings were 80, 83, 85, and 81, Manchester United’s defense rating would be the integer average of these four ratings, which is 82. The match outcome was defined as 0 for a loss, 1 for a draw, and 2 for a win, and the classifier would output one of these three numbers given the data. After training the model with 70% of the data set, the models accuracy was tested using the remaining 30% of the data set. The model was able to predict the match outcomes with an accuracy of 73.33%. 
