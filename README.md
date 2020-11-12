# Capstone 2

## Proposal 1 - Simpsons Episode Quality Predictor

In my teenage years, I loved the television show The Simpsons. As I got older, I agree with most of the rest of the world that as the Simpsons aged, the show quality declined. However that doesn't diminish the quality of the show in its early years. Using a data set I found online, I would like to look at what made a higher quality Simpsons episode.

Some of the features include:

* IMDB rating, air date, title, number of viewers
* Spoken dialogue by each character in the episode
* Locations (settings) appearing in the episode


* [The Simpsons by the Data](https://data.world/data-society/the-simpsons-by-the-data)

Aditionally, depending on what I learn with NLP, if it is possible I would also like to look at how the dialogue relates to th episode quality as well. Were certian lines, jokes, or topics associated with episode rating?

## Proposal 2 -  World Cup success predictor

I am a HUGE international soccer fan and the World Cup is about as close as I can get to heaven. The data found [here](https://zenodo.org/record/1935382#.X6ydd65MFhEI) gives deep nsight to player level performance during each world cup match. Therefore, I would like to do an analysis on the player performance during games and attempt to identify, at the player level, what determines success in a World Cup match. I would like to look at two outcomes:

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