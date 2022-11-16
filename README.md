# TITLE

#### Abstract: A 150 word description of the project idea and goals. What’s the motivation behind your project? What story would you like to tell, and why?
Did you know that former President Barack Obama was the first president ever to brew a beer in the White House ? The US was ranked 15th 

**Are US people subject to give better grades for local beers? Do people prefer their state's beers?**

#### Research Questions: A list of research questions you would like to address during the project.

To address this question we should also consider answering the followings : 
- Are some states/cities more represented than others ? 
- Are the most consumed beers also the ones with a greater number of rating ?
- Are the preferred foreign beers similar to the preferred local beers —> is there a preferred type of beer for the region ?
- How politics tendencies are spread within USA ? And can we observe trends in beer consumption related to this politics tendencies ? 

To answer main idea : 
How many countries have a national beer as a top beer/in the top X beers (LINK TO SUB IDEA ABOUT MOST CONSUMED BEERS)
compare that ratio to the ratio of people that drink beers/ liter of beer drank per year in each country
Find the ratio of national and foreign beers in the top X beers in each country

#### Proposed additional datasets (if any): List the additional dataset(s) you want to use (if any), and some ideas on how you expect to get, manage, process, and enrich it/them. Show us that you’ve read the docs and some examples, and that you have a clear idea on what to expect. Discuss data size and format if relevant. It is your responsibility to check that what you propose is feasible.



#### How are the Data handled ?

Our datasets are named **RateBeer.tar.gz**, **matched_beer_data.tar.gz** and **BeerAdvocate.tar.gz**. These are compressed folders containing both csv and txt files. In order to ease our analysis we created different methods to create this tree structure : 

![image](data_structure.png)

#### Methods

We loaded the BeerAdvocate and RateBeer datasets for years 2001-2017. We converted the txt files into csv and compressed them back. These files are now stored into our local machines to optimize storage. We processed the data by removing every line missing an argument to have a global vision of the dataframes we could work with.
We created two different dataframes, one for each site, merging all the data we considered useful for further analysis.

### **Data description**

| Column name          | Description                                                                                                                                                                                       |   |   |   |
|----------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---|---|---|
| beer_id           | The beer ID                                                                                                                                                 |   |   |   |
| beer_name            | The beer name                                                                                       |   |   |   |
| brewery_id | The Brewerie name                                                                                                                     |   |   |   |
| brewery_name          | The brewery name   |   |   |   |
| style             | Beer style (e.g. English Brown Ale, Indian Pale Ale, Kölsch)                                                                                                                                                                  |   |   |   |
| nbr_ratings        | The number of ratings made for this beer ID                                                                                          |   |   |   |
| nbr_reviews               | The number of reviews made for this beer ID                                     |   |   |   |
| avg              |                                                                                                                                                                                 |   |   |   |
| ba_score or rb_score                 | Numeric value attributed to the beer ID                                                                                                                                                    |   |   |   |
| bros_score                 | ??                                                                                                                                                               |   |   |   |
| abv           | Alcohol by volume, standard measurement, used worldwide, to assess the strength of a particular beer.                                                  |   |   |   |
| avg_computed               |                                                                                                                      |   |   |   |
| zscore         |  |   |   |   |
| nbr_matched_valid_ratings          | Along with significance, shown to editors to guide decisions about what test to choose                                                                                                            |   |   |   |
| avg_matched_valid_ratings               | Whether a package was selected by editors to be used on the Upworthy site after the test                                                                                                          |   |   |   |



Furthermore we load an additional dataset containing the persons present in the Quotebank dataset as a speaker. For the persons in the Quotebank dataset the second dataset contains the following for each person: Wikidata QID, full name, list of aliases. These aliases will turn very usefull in later stages of the project to detect persons being mentioned in quotes.

#### Proposed timeline

Before November 18th :
- Data processing, visualization, creation of a dataframe containing all the information extracted from every file for each website.
- Creation of a new column containing the States name imported from Wikipedia to plot correctly a world map.
- Interactive mapping of the different beer locations and users locations, worldwide and USA centered

Before December 2d :
- Homework 2 
- Sentimental analysis of the reviews to see whether they corresponds to a positive or negative sentiment. Furthermore, we will perform emotional analysis to see the evolution of particular emotions throughout different reviews of a same user. 

Before December 16th :
- Principal Components Analysis (PCA) keeping 2 of the 4 beer aspects 
- Analysis of correlations between users nationalities and beer production locations
- Random forest of 10’000 trees trained to find the optimal combination of aspects
- Meaningful plots to complement the interactive maps

Before December 23d :
- Story-telling 
- Github repository cleaning and organisation
- README completion

#### Organization within the team
| Thibault | Claire | Mathis | Achraf |
|---|---|---|---|
| Politic tendencies dataset handling and processing  | Data handling | Geographical correlations | Data cleaning/filtering |
| Time Series Analysis | Sentimental analysis of reviews | Random forest training | Plot interractive US maps  |
| Data Story (20%)  | Data Story (40%) | Data Story (20%) | Data Story (20%) |

#### Questions for TAs (optional): Add here any questions you have for us related to the proposed project.

