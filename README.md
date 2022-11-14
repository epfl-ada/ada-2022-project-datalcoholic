# TITLE

#### Abstract: A 150 word description of the project idea and goals. What’s the motivation behind your project? What story would you like to tell, and why?

**Are US people subject to give better grades for local beers? Do people prefer their state's beers?**

#### Research Questions: A list of research questions you would like to address during the project.

To address this question we should consider answering these too : 
- Are some states/cities more represented than others ? 
are the most consumed beers also the ones with a greater nb of rating (correlation, see for most consumed and most rated beers, inner join with data from other source)
are the preferred foreign beers similar to the preferred local beers —> is there a preferred type of beer for the region ?
Local beer is probably the most drank in a region but is it the most liked (better rate)
US, politics tendencies


To answer main idea : 
How many countries have a national beer as a top beer/in the top X beers (LINK TO SUB IDEA ABOUT MOST CONSUMED BEERS)
compare that ratio to the ratio of people that drink beers/ liter of beer drank per year in each country
Find the ratio of national and foreign beers in the top X beers in each country

#### Proposed additional datasets (if any): List the additional dataset(s) you want to use (if any), and some ideas on how you expect to get, manage, process, and enrich it/them. Show us that you’ve read the docs and some examples, and that you have a clear idea on what to expect. Discuss data size and format if relevant. It is your responsibility to check that what you propose is feasible.

#### How are the Data handled ?

Our datasets are named **RateBeer.tar.gz**, **matched_beer_data.tar.gz** and **BeerAdvocate.tar.gz**. These are compressed folders containing both csv and txt files. In order to ease our analysis we created different methods to create this tree structure : 

![image](data_structure.png)

At the end the newly created compressed files are stored on our own machine and the notebooks use the same tree structure with the Data folder at the same level than the repository.

#### Methods

For the RateBeer dataset, the ratings.txt.gz and reviews.txt.gz files are the same and correspond to the latter, we thus do not take the former in our analysis.

#### Proposed timeline

#### Organization within the team: A list of internal milestones up until project Milestone P3.

#### Questions for TAs (optional): Add here any questions you have for us related to the proposed project.

