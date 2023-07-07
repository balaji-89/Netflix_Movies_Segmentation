# Netflix_Movies_Segmentation
An Unsupervised ML Capstone Project
Problem Statement:
This dataset consists of tv shows and movies available on Netflix as of 2019. The dataset is collected from Flixable which is a third-party Netflix search engine.
We need to do:
1) Exploratory Data Analysis.
2) Understanding what type of content is available in different countries.
3) Is Netflix increasingly focusing on TV rather than movies in recent years?
4) Clustering similar content by matching text-based features.
   
![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

   ![image](https://github.com/balaji-89/Netflix_Movies_Segmentation/assets/57706260/a5190601-dc65-4de1-a190-2935e7719303)

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

WHAT I DID?

The first step I did after importing the dataset is knowing the basic information about the dataset. 
After that, I planned the Data Wrangling part and Data preprocessing steps. First I converted a date feature that is by default loaded as the object to pandas datetime object so that I can use that feature easily for future purposes as datetime object gives many predefined methods to specifically work with date.
Next, I didn't handle the missing values in the dataset, because the missing data appeared in some features with less in numbers so we can use that for EDA which doesn't make any difference. Next thing is I going to use the text-based feature that is "Description" for training machine learning model. These are the reason behind of not handling the missing values.
The next step is text preprocessing, before making this feature into a meaningful multi-dimensional vector, I need to do some preprocessing steps which are changing to lowercase, then removing punctual, stopping words and extra white spaces, etc.

Finally, I used the TfidVector to change the text data into numerical, I chose 400 as the maximum features so each review observation will be converted into 400 length features.

Then after converting this vector, the next step is building clustering machine learning models. I tried three different models, the first one is K-means, then I tried Hierarchical Clustering, and finally DBSCAN algorithm.

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

## Library Used:
  - Pytorch
  - Numpy
  - Pandas
    
![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

## Execution Instructions:

1. Clone the repository:

   ```
   git clone https://github.com/balaji-89/Netflix_Movies_Segmentation.git
   ```


2. Run :
      open file under src/netflix_clustering.ipynb, then run it cell by cell
   
Feel free to modify and adapt the content according to your project's specific details and requirements.


