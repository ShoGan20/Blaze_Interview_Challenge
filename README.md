# Blaze_Interview_Challenge
 Obtain 1000 follower details and perform Classification on it.

-----------------------------------------------------------------------------------------------------------------------------------------

Methodology:

	1. Used the twitter API OAuth V1.1 to obtain 1000 follower details of user 'open sea'
	2. Details contain: Screen name, Follower count, Verified, Following count, Location, Description
	3. Stored the data into a csv file using pandas
	4. Performed some visualisations to gain insights on the dataset
	5. Applied feature engineer such as Cleaning Description Column, Calculating follows to follower count ratio, Converting Verified column Boolean to 1, 0 values
	6. Used TF-IDF Vectorization on textual data and standard scalars for the other columns
	7. Applied Random Forest Classification on dataset
	8. Evaulated using precision score, recall score and f1-score

-----------------------------------------------------------------------------------------------------------------------------------------

Some thoughts on the challenge:

	1. I think the data set is too small hence the predictions are really good.
	2. Just using follower count, following count, location and Description is not good enough as samples
	3. These values dont seem to hold a lot of influence in the predcition of verification.
	4. To improve, we could try using the tweets of the user and applying Sentiment Analysis on it.
	5. I tried using SMOTE and imblearn to help with the prediction but data was too small for that.
	6. If given more time, I could use some better feature engineering methods and play with the hyper parameter

 