# Capstone 3

## Proposal 1 - Using NLP to determine the type of genetic variants in tumors

Cancer is born from mutations in our DNA. DNA codes for proteins that perform specific tasks in our bodies. When DNA gets mutated, say from cigarette smoke or a sunburn, the protein produced by that strand of DNA may be altered, and thus become a variant (or mutation). The protein that is coded from that DNA may be altered as well, and there are several different potential classifications for these alterations. Luckily, the names of the alterations are fairly self-explanatory.

* Gain-of-function - the protein gains a new ability that it did not previously have (this can cause cancer if the new function promotes rapid cell division and growth).
* Loss-of-function - the protein loses it's ability to perform a function (we have proteins, like p53, whose job is to slow down cell division and if that function is lost, cancer is more likely to develop).
* Switch-of-function - a protein may change what it does (similar possibilities as described above).
* Neutral - the genetic code is degenerate, meaning there are multiple ways to code out similar proteins. Therefore, it is also possible for a variant to simply be neutral and not cause any issues at all.


Even within the last 5 years, in order to classify an alteration in a gene (variant) a pathologist would have to choose a variant of interest, identify medical literature that is relevant to the variant of interest, and then study the evidence to classify the variation. This process is very time consuming. In order to speed up the process, Kaggle released a data set meant for designing a machine learning model that would analyze evidence and literature about a specific tumor gene alteration, and classify it into one of 9 types of alterations. I would like to use this data to create my own model to classify the genetic variants.

The data set is located [here](https://www.kaggle.com/c/msk-redefining-cancer-treatment/data). I will be using the training_text, training_variants, test_text, and test_variants data sets.

The text data contains the ID and the literature evidence to be used to classify the variation

The variants data features are:
* ID
* Gene
* Variation
* Class (target variable)

The class variable is on a scale ranging from 1 to 9 for each class. Kaggle did not provide the breakdown of what each class is. To find this out, I went to the [OncoKB](https://www.oncokb.org/) website, which contains a library of the types of variations and can identify the class of each variant. By plugging some of the variants into the data base I was able to determine the following breakdown of the classes:

1. Likely loss-of-function
2. Likely gain-of-function
3. Neutral
4. Loss-of-function
5. Likely neutral
6. Inconclusive
7. Gain-of-function
8. Likely change-of-function
9. Change-of-function

<hr>

# Capstone 2

## Proposal 1 - Breast Cancer Identification

Cancer has always been a fascination of mine. I did my Master's Degree on disease free survival from Ductal Carcinoma in situ, a form of non-malignant breast cancer. I would love to continue working in a field of chronic or infectious diseases one day.  As such, I would like to take this [dataset](https://www.kaggle.com/paultimothymooney/breast-histopathology-images) of over 250,000 breast histopathology images, I would like to build a model that can detect images of invasive breast cancer.

I believe this project would be both challenging but very rewarding for me as well

## Proposal 2 -  World Cup success predictor

I am a HUGE international soccer fan and the World Cup is about as close as I can get to heaven. The data found [here](https://zenodo.org/record/1935382#.X6ydd65MFhEI) gives deep insight to player level performance during each world cup match. Therefore, I would like to do an analysis on the player performance during games and attempt to identify, at the player level, what determines success in a World Cup match. I would like to look at two outcomes:

1. The probability of winning a particular match based on the player level data
2. Predicting what round a team is likely to reach based on aggregate data at the player level.

A couple examples of the player level data:

* Passes Completed
* Distance covered in possession
* Sprints
* Shots
* Saves
* Fouls
    * Yellow and Red cards
* Time spent in certain locations on the field.
    * E.g. if defenders are in the attacking third more often that's probably good while if attacking players are spending lots of time in their defensive zone that's probably a bad sign.

I intend to use the South Africa and Brazil World Cup data to create the models as that is more complete. The less complete Russia data may serve as a good test data set for predicting matches and tournament progression

## Proposal 3 - More Breast Cancer Diagnostics

Using data from the Breast Cancer Wisconsin Diagnostic Data set found [here](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+%28Diagnostic%29), I would like to build a model to predict malignant breast cancer diagnoses. Some features included are

a) radius (mean of distances from center to points on the perimeter)
b) texture (standard deviation of gray-scale values)
c) perimeter
d) area

Other features of cell nucluei are included in the dataset, but only 10 or so I am not sure how we feel about that.

<hr>

# Capstone 1

## Proposal 1 - Lung Cancer Mortality Across the United States

 I would like to scrape the CDC Wonder website to compare mortality rates due to lung cancer across the regions of the United States. My hypothesis will be that each region (West, Midwest, etc) has equal death rates due to lung cancer. Time permitting, I would also like to compare across regions by age, race, and gender.

* Features
    * State
    * 5-year age group
    * Sex
    * Race
    * Ethnicity
    * Deaths
    * Population

* [US Lung Cancer Morality 2008-2017](https://wonder.cdc.gov/controller/saved/D161/D94F276)


## Proposal 2 - Are Classic Books rated higher?

I love a good book. I would like to scrape the top books that everyone should read according to Goodreads. Are these books that Goodreads thinks I should read rated higher? My hypothesis would be that higher ranked books in the list are not rated higher on average than the lower ranked books. Additionally I would like to investigate these books based on their length and release date as well.

* Features
    * Ranking
    * Rating
    * Publication year
    * Pages

* [Goodreads Books Everyone Should Read](https://www.goodreads.com/list/show/264.Books_That_Everyone_Should_Read_At_Least_Once)