<h1 align="center"> Play Store App Review Analysis</h1>
<h3 align="center"> AlmaBetter Verfied Project - <a href="https://www.almabetter.com/"> AlmaBetter </a> </h5>

<p align="center"> 
<img src="GIF/google play.gif" alt="Animated gif" height="282px">
</p>

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

## 📋 Abstract
A few thousand new applications are regularly uploaded to the Google Play Store. A huge number of designers working freely on designing the apps and making them successful. With the enormous challenge from everywhere throughout the globe, a developer needs to know whether he/she is continuing the correct way or not. Since most Play Store applications are free, the income model is very obscure and inaccessible regarding how the in-application buys, in-application adverts, and memberships add to the achievement of an application. In this way, an application's prosperity is normally dictated by the quantity of installation of the application, and the client appraisals that it has gotten over its lifetime instead of the income created.
The objective of this experiment is to deliver insights to understand customer demands better and thus help developers popularize the product. We have tried to discover the relationships among various attributes such as which application is free or paid, what are the user reviews, rating of the application.
![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

##  💾 Project Files Description

<p>This Project includes 1 colab notebook and 1 technical documentation</p>

### Executable Files:
- [Play Store App Review Analysis](https://github.com/Parag-A/Play-Store-Review-Analysis/blob/main/Play_Store_App_Review_Analysis_.ipynb) - Includes all functions required for clustering operations.

### Output:
- [Google Colab](https://github.com/Parag-A/Play-Store-Review-Analysis/blob/main/Play_Store_App_Review_Analysis_Output.ipynb) - All the outputs are visible in the provided colab notebook.

### Input Files:
  <li><b>Play Store Data.csv</b> - It contains the basic details of the app like the number of user reviews, ratings, etc.</li>
  <li><b>User Reviews.csv</b> - It contains the user reviews and its sentiment score for the respective app.</li>

### Data Source:
- [Dataset](https://learn.almabetter.com/courses/take/team-capstone-projects/texts/19443175-play-store-app-review-analysis-dataset) - Dataset taken from Almabetter

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

## 📖 Introduction:
In today’s scenario, we can see that mobile apps play an important role in any individual’s life. With enormous challenges from everywhere throughout the globe, a designer needs to realize whether he/she is continuing in the right way or not. To hold this income and their place in the market the application designers may need to figure out how to stick to their present position.
The dataset with 10k Play Store applications is available to analyze the market of android. It can be examined to analyze the different categories such as family, communication, entertainment, tools, music, camera, etc. In this project, we examine the different attributes present in the data set that affect the popularity of the application. We focused on to answer questions like, what makes an app popular, what should be the price and size of the app, is there some trends in user sentiments. 
In our data set, we have two CSV files for data analysis:
Play Store data
User Reviews
At first, we analyzed the Play Store data and in the Play Store data we have 10841 rows and 13 columns & in the user review data, we have 64295 rows and 5 columns of data. We have to take the maximum outcomes from the data which helps us to analysis which type of app is most preferable and comparisons between different insights. Our goal is to filter and make plots accordingly for a better EDA concerning the final data. We need to explore and analyze the data to discover key factors responsible for app engagement and success. 

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
### The contents of Play Store Data are:
* App: It contains the name of the app with a short description (optional).
* Category: This section gives the category to which an app belongs. In this dataset, the apps are divided among 33 categories.
* Size: The disk space required to install the respective app.
* Rating: The average rating given by the users for the respective app. It can be in between 1 and 5.
* Reviews: The number of users that have dropped a review for the respective app.
* Installs: The approximate number of times the respective app was installed.
* Type: It states whether an app is free to use or paid.
* Price: It gives the price payable to install the app. For free type apps, the price is zero.
* Content rating: It states which age group is suitable to consume the content of the respective app.
* Genres: It gives the genre(s) to which the respective app belongs.
* Last updated: It gives the day in which the latest update for the respective app was released.
* Current Ver: It gives the current version of the respective app.
* Android Ver: It gives the Android version of the respective app.

### The contents of User Reviews are:
* App: It contains the name of the app with a short description (optional).
* Translated_Review: It contains the English translation of the review dropped by the user of the app.
* Sentiment: It gives the attitude/emotion of the writer. It can be ‘Positive’, ‘Negative’, or ‘Neutral’.
* Sentiment_Polarity: It gives the polarity of the review. Its range is [-1,1], where 1 means ‘Positive statement’ and -1 means a ‘Negative statement’.
* Sentiment_Subjectivity: This value gives how close a reviewer’s opinion is to the opinion of the general public. Its range is [0,1]. Higher the subjectivity, closer is the reviewer’s opinion to the opinion of the general public, and lower subjectivity indicates the review is more of a factual information.

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

## 📋Problem Statements
1. What are the top categories on Play Store?
2. Are the majority of the apps Paid or Free?
3. How important is the rating of the application?
4. Which categories from the audience should the app be based on?
5. Which category has the most no. of installations?
6. How does the count of apps vary by Genre?
7. How does the last update has an effect on the rating?
8. How are ratings affected when the app is a paid one?
9. How are reviews and ratings co-related?
10. Let us discuss the sentiment subjectivity.
11. Is subjectivity and polarity proportional to each other?
12. What is the percentage of review sentiments?
13. How is sentiment polarity varying for paid and free apps?
14. How does Content Rating affect the App?
15. Does the Last Update date have an effect on the rating?
16. Distribution of App updates over the Year.
17. Distribution of Paid and Free app updated over the Month.

********************************************************************************************************************************************************************
## 📔 **What is Exploratory Data Analysis?**
Exploratory data analysis (EDA) is used by data scientists to analyze and investigate data sets for patterns, and anomalies (outliers), and form hypotheses based on our understanding of the dataset and summarize their main characteristics, often employing data visualization methods. It is an important step in any Data Analysis or Data Science project. It helps determine how best to manipulate data sources to get the answers you need.

EDA involves generating summary statistics for numerical data in the dataset and creating various graphical representations to understand the data better and make it more attractive and appealing.

The following are the various steps involved in the EDA process:
1. <b>Problem Statement</b> - We shall brainstorm and understand the given data set. We shall study the attributes present in it and try to do a philosophical analysis of their meaning and importance for this problem.
2. <b>Hypothesis</b> - Upon studying the attributes present in the database, we shall develop some basic hypotheses on which we can work and play with the data to look for the varied results that we can get out of it.
3. <b>Univariate Analysis</b> - It is the simplest form of analyzing the data. In this we would initially pick up a single attribute and study it in and out. It doesn't deal with any sort of co-relation and it's major purpose is to describe. It takes data, summarizes that data, and finds patterns in the data.
4. <b>Bivariate Analysis</b> - This analysis is related to the cause and the relationship between the two attributes. We will try to understand the dependency of attributes on each other.
5. <b>Multivariate Analysis</b> - This is done when more than two variables have to be analyzed simultaneously.
5. <b>Data Cleaning</b> - We shall clean the dataset and handle the missing data, outliers, and categorical variables.
6. <b>Testing Hypothesis</b> - We shall check if our data meets the assumptions required by most of the multivariate techniques.

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

## 📖	Steps Involved
After loading the dataset, we can start the exploration but before that, we need to check and see whether the dataset is ready for performing several exploration operations or not, so let’s first have a look at the structure and the manner in which the data is organized.

### Data Cleaning
Our data set contains a large number of null values in the rating column, so we drop them. Some of the columns have a smaller number of null values, so we replace the null values in these columns with the mode value of that particular column. Our data set also contains duplicate rows for a single application. We also drop the duplicate rows because the rows contain identical data. Also drop the rows, which have ratings greater than 5.

### Data Transforming 
From the information of data frame, we can see that all the columns except rating have the object data type but some of the columns like, reviews, size, installs, and price have the numerical value. So, we have to transform them into proper data type and also remove the unwanted values from the numerical columns like ‘+’ and ‘,’ from installs and ‘$’ from price. In the size column, we have some values in KB and some values in MB, so we transform all the values in MB.

### Exploratory Data Analysis
After establishing a good sense of each feature, we proceeded with plotting a pairwise plot between all the quantitative variables to look for any evident patterns or relationships between the features. There is a high variance in the number of installs and in a number of reviews. To overcome this problem, we add two new columns to the data frame named: log_installs and log_review, which contain the logarithmic values of installs and review columns, respectively.

### Single Variate Analysis
After that, we analyzed all the columns one by one to examine whether the particular column contained some useful information or not:

### Category
We break down the apps by category and observe that family and game categories have the maximum number of apps in the Play Store. Weather, house and home, comics, events, beauty, and parenting are the categories that have a few numbers of apps.

### Data wrangling
Apart from this, two new columns were added to the main data frame, namely, “Rating Group”, and “Revenue”. This is done to improve and simplify the analysis and come up with different meaningful visualizations

* <b>Rating Group:</b> This column groups the apps based on the average user rating. (4-5: Top rated, 3-4: Above average, 2-3: Average, 1-2: Below average).
*	<b>Revenue:</b> This column gives the revenue generated by the app through app installs alone.
By doing these operations on the original dataset, we are ready with the data pipeline, and data visualizations can be done on it.
All the apps in the Play Store have ratings between 0.5 and 5. Maximum apps have a rating between 3.8 and 4.5.

### Installs
We analyzed the install column to observe the effect of size, price, rating, content rating, android version on app installation number. We can analysis that for each and every category number of app installations does not depend on the size. The free apps are installed mostly. The apps which can be used by everyone is more installed than the apps which can be used by a particular age group. The rating of mostly installed apps is between 4 and 5.

## 🛠	Challenges Faced:
* Reading the dataset and comprehending the problem statement. Our major challenge was data cleaning.
* Handling the error, duplicate, and NaN values in the dataset.
* 13.60% of reviews were NaN values, and even after merging both data frames, we could not infer much in order to fill them. Thus we had to drop them.
* The merged data frame of both play store and user reviews, had only 816 common apps. This is just 10% of the cleaned data, we could have given a more valuable analysis, if we had at least 70% - 80% of the data available in the merged data frames.
* User Reviews had 42% NaN values, which could have been used for developing an understanding of the category-wise sentiments, which would help us to fill 13.60% NaN values of the Reviews column.
* There is so much more that can be explored. Like we have the current version, android version available which can be explored in detail and we can come out with more analysis where we can tell how these things effect and need to be kept in mind while developing an app for the users.
* We can explore the correlation between the size of the app and the version of Android on the number of installs.
* Machine learning can help us to deploy more insights by developing models that can help us interpret even better. We have left this as future work as this is something where we can work on.
*	Designing multiple visualizations to summarize the information in the dataset and successfully communicating the results and trends to the reader.

## 📋 Conclusion:
Most of the apps are free so developers should focus on creating free apps to have a huge customer base. If developing paid apps then apps size should not be greater than 40 MB. More Apps should be in the category of Events, Beauty, and Parenting as they have not been explored much but are still quite popular with huge installations. In order to retain the customer base apps should be updated regularly Developers should develop apps such that their content is available for everyone. Bulky apps should be developed in categories like Game, Family. If developing paid apps then its price should not be high and the size should be less than 20 MB. Apps belonging to the Game and Family Category have high negative reviews therefore they should be developed carefully. Like this, there can be a lot of conclusions but we have tried to cover the most important ones.
These are some of the aspects that the developer should research before proceeding with the app development. By conducting a simple exploratory data analysis (EDA) on the Play Store dataset, we not only eliminate avoidable risks of failure, but we may also be able to provide better ideas for building the app.
*	Percentage of free apps = ~92%
*	Percentage of apps with no age restrictions = ~82%
*	Most competitive category: Family
*	Category with the highest number of installs: Game
*	Category with the highest average app installs: Communication
*	Percentage of apps that are top rated = ~80%
*	There are 20 free apps that have been installed over a billion times
*	Minecraft is the only app in the paid category with over 10M installs. This app has also produced the most revenue only from the installation fee.
*	Category in which the paid apps have the highest average installation fee: Finance
*	Most popular app in the Play Store based on the number of reviews: Facebook
*	The median size of all apps in the Play Store is 12 MB.
*	The apps whose size varies with the device has the highest number of average app installs.
*	The apps whose size is greater than 90 MB have the highest number of average user reviews, i.e., they are more popular than the rest.
*	Helix Jump has the highest number of positive reviews and Angry Birds Classic has the highest number of negative reviews.

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

## 💶 Credits

Contact me for Data Science Project Collaborations

[![GitHub](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://github.com/San13deep)
[![LinkedIn](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/paragsagrawal/)

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

## 📚 References
*	GeeksforGeeks
*	Analytics Vidhya
*	Stackoverflow
*	Towards data science
*	Python libraries documentation
*	Data camp

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
## 📜 Feedback
If you have any feedback, please reach out to us at agrawalparag9921@gmail.com

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

