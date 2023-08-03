# Machine-Learning-Project--Sleep-health-and-lifestyle
A dataset pertaining to sleep health and lifestyle is subjected to a data analysis and classification task using this code. It makes use of a number of Python ecosystem libraries, encompassing numpy, pandas, matplotlib, seaborn, and scikit-learn. The following actions are taken by the code:
## Step 1 - Exploratory Data Analysis (EDA):
The programme starts by importing the required libraries and extracting the dataset from a CSV file with the file extension "Sleep_Health_and_Lifestyle_Dataset.csv." subsequently basic dataset details like the data types and non-null counts for each column are printed. The 'describe()' method is also used to display an overview of statistical measurements for numeric columns. The dataset has 374 rows and 13 columns with objects (strings), integers, and floats among other data types.

## Step 1 (continued) - Data Visualization:
Following the first data investigation, the algorithm use seaborn to provide data visualisations. The dataset's correlations between various numerical variables, classified by the "Sleep Disorder" feature, are first visualised using a pair plot. Each graphic demonstrates the relationships between several variables and the distribution of data points according to various sleep disorders.

Furthermore, The correlation matrix between the dataset's numerical characteristics is then shown as a heatmap. Colours are used in the correlation heatmap to show the direction and degree of the link between features. The code also inserts numerical numbers to display the correlation coefficients within every cell. 

## Step 2 - Data Pre-processing:
To maintain the original data, the code generates a copy of the original dataframe named "df1" in this phase. The categorical variables are subsequently transformed into numeric values using labelled encoding. Occupation, Gender, BMI Category, Blood Pressure, and Sleep Disorder are the columns that are being encoded.

The algorithm eliminates a number of columns that are assessed unnecessary for the categorization operation after encoding the category columns. BMI Category, Gender, Person ID, Stress Level, Blood Pressure, and Heart Rate are the columns that are being removed.

## Step 2 (continued) - Data Visualization after Encoding:
Afterwards,  pre-processing the data, the algorithm creates fresh visualisations to investigate connections among the characteristics and the intended variable, "Sleep Disorder." To display the encoded characteristics and their correlations with the target variable, it generates another pair plot and a correlation heatmap.

## Step 3 - Feature Selection:
In this stage, the code divides the characteristics from the target variable "Sleep Disorder" and assigns them to X and y, accordingly. This is a standard machine learning strategy where the target variable is used for prediction while the characteristics are utilised to train the model.

## Model Explanation:
### K-Nearest Neighbors (KNN)
A straightforward and user-friendly supervised machine learning technique called K-Nearest Neighbours (KNN) is employed for classification and regression applications. The fundamental goal of KNN is to categorise a data point based on the feature space's k closest neighbours' predominant class. In other words, it makes the assumption that comparable data points are probably members of the same class.

KNN's basic operating premise is as follows:
Data Collection
Distance Calculation
Selecting K
Voting and Classification
Evaluation

It's important to note that KNN is a non-parametric and lazy learning algorithm, which means it doesn't make any assumptions about the distribution of the underlying data and doesn't build an explicit model during training. Instead, the complete dataset is stored, and calculations are made when a prediction is made. While KNN is straightforward and simple to use, its computational cost can drastically rise with big datasets, making it less appropriate for real-time applications or high-dimensional data. KNN is still a useful and popular approach, especially for smaller datasets and as a comparison tool for more advanced machine learning models.

Training data to the KNN model using the `fit()` function, which trains the model based on the provided data.
