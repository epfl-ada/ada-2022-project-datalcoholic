# TITLE

- Abstract: A 150 word description of the project idea and goals. What’s the motivation behind your project? What story would you like to tell, and why?

- Research Questions: A list of research questions you would like to address during the project.

- Proposed additional datasets (if any): List the additional dataset(s) you want to use (if any), and some ideas on how you expect to get, manage, process, and enrich it/them. Show us that you’ve read the docs and some examples, and that you have a clear idea on what to expect. Discuss data size and format if relevant. It is your responsibility to check that what you propose is feasible.

- How are the Data handled ?

Our datasets are named **RateBeer.tar.gz**, **matched_beer_data.tar.gz** and **BeerAdvocate.tar.gz**. These are compressed folders containing both csv and txt files. In order to ease our analysis we created different methods to create this tree structure : 

![image](data_structure.png)

At the end the newly created compressed files are stored on our own machine and the notebooks use the same tree structure with the Data folder at the same level than the repository.

- Methods

For the RateBeer dataset, the ratings.txt.gz and reviews.txt.gz files are the same and correspond to the latter, we thus do not take the former in our analysis.

- Proposed timeline

- Organization within the team: A list of internal milestones up until project Milestone P3.

- Questions for TAs (optional): Add here any questions you have for us related to the proposed project.

