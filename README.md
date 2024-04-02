# Twitter-Aggression-Analysis
Summary : Performed classification &amp; Analysis on Scraped Twitter data based on aggressiveness using machine learning models. Performed Scraping, pre-processing and selecting a suitable algorithm for training of Trac1 dataset. Multinomial NB model was then tested, analyzed for performance &amp; classification of scraped data was done.

# Process Used for the project:
# Step 1: Data Extraction
We utilized the'snscrape' package to extract data about the topics listed above. Users can extract data from Twitter by utilizing search queries. The library makes it easy to extract massive volumes of data from Twitter, making it an excellent tool for social media research. A search query is supplied to extract Data, which might include hashtags, dates, and other criteria. We added keywords between particular dates in our search query for our study project and extracted Tweet Date, Tweet Username, Tweet Content, Tweet User Location, Tweet User Profile Description, Tweet Retweet Count, and Tweet User Follower Count. This data is then transformed into a structured data format, such as a Pandas Dataframe, for further analysis

# Step 2: Loading and pre-processing the dataset
Using regular expressions, the dataset was pre-processed by eliminating special characters and punctuation and converting all text to lowercase. This stage is critical since it aids in the preparation of the data for feeding to the machine learning model.

# Step 3: Text data vectorization
Text data is transformed into numerical data. TfidfVectorizer is utilized since it is one of the most popular and efficient methods for converting text input to numerical form.

# Step 4: Splitting the data
The dataset is divided into two parts: training and testing. Splitting the data aids in evaluating the model's performance on previously unseen data. It also aids in the prevention of overfitting, which occurs when the model becomes too complicated and begins to learn the noise in the data.

# Step 5: Defining the classification models
A set of classification models to be trained and assessed is provided, which includes the Random Forest Classifier, Linear SVC, Multinomial Naive Bayes, and Logistic Regression. Each of these models has advantages and disadvantages, and comparing them allows you to choose the ideal one for the job.

# Step 6: Training and evaluating the models
The for loop iterates through each model, trains it on training data, predicts labels for both training and testing datasets, and computes accuracy scores for both datasets. The accuracy score indicates how effectively the model is performing. If the accuracy score is low, it indicates that the model is underperforming and should be improved.
