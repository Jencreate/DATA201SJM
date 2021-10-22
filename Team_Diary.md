#### Entry (20/09/21) - Team
- Attempted to generate ideas for the assignment topic (17/09/21) (see vocabulary_game.md)
  - Each team member created a list of random words of any topic.
  - The words from each member were combined to form multiple sentences relating to a topic idea.
  - The ideas were further refined to meet the context of the assignment.

#### Entry (24/09/21) - Team
- New team member in group, Liyinqin Li. SJM now has a group size of 4.
- 'energy production by river flow with rainfall' was chosen as the first topic for prototyping.
  - We found data for energy production by hydrostation, with the corresponding river flow data.
  - We could not find sufficient rain fall data over a long period of time for the locations of the hydrostations.  
- Changed our topic to our second choice 'energy production by riverflow with electricity cost' due to the above reason.

#### Entry (01/10/21) - Team
- Found the data sets for power production by hydrostations, river flow, and electricity cost.
- Decided to use 2020 data for each of the above datasets as it was available for each subject.
- The data retrieval and wrangling must be done automatically, and so scripts will have to be created to handle the automatic process.
- Created and updated the team plan to assign tasks to individual members.
    - Each individual member should create an R script to webscrape their subject's data from their respective sources. 

#### Entry (01/10/21) - Jensen
- I will create a python script to convert xlsx/xls files to csv so the data contained within may be easily wrangled in R.

#### Entry (01/10/21) - Matt
- With help from Giulio, figured out a way to create a sort of manual api from a download url.
- Found url changes when using different datasets from the niwa website and obtained the different values required for my rivers.

#### Entry (07/10/21) - Jensen
- Perhaps R has a package that will allow the conversion of xlsx/xls to csv. I will aim to use such a package instead. 
- 
#### Entry (07/10/21) - Sujung
- Convert excel file from web in R directly

#### Entry (08/10/21) - Team
- Spent most of time collaborating with another group, sharing our projects.
- Attempted to fix github issues regarding merging repositories.
- Compared hydrostations and the river flows of the rivers they reside on.

#### Entry (08/10/21) - Sujung
- Remove unnecessary data and organize the necessary data for comparing with other data.

#### Entry (10/10/21) - Jensen
- Identified the coordinates of each appropriate hydrostation and created a tibble containing this data.

#### Entry (13/10/21) - Matt
- Used Jensens hydrostation data to figure out which rivers/lakes they are on and for each, what data i can find on the aquarius portal

#### Entry (15/10/21) - Richard
- Beginning write the report about this project.

#### Entry (15/10/21) - Team
- After comparing the river flow data with the hydrostation fleet location information, we found the greatest level of accuracy to be by month. This presented us with only 11 data point for each hydrostation, as the river flow data for April was missing aswell. For this reason, we have decided to extend the range of our data to multiple years.
- Furthermore, only 11 out of the 47 hydrostations identified contained useable river flow data from the source used.

### Entry (22/10/21) - Matt
- Have made a few changes over the past days to my river notebook, nearly ready for combination with jensen's data, need to remove part of time rows

### Entry (22/10/21) - Team
- finalising data, almost ready to start combining and then graph some data, starting work on presentation