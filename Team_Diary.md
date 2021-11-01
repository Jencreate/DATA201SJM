#### Entry (20/09/21) - Team
- Attempted to generate ideas for the assignment topic (17/09/21) (see vocabulary_game.md)
  - Each team member created a list of random words of any topic.
  - The words from each member were combined to form multiple sentences relating to a topic idea.
  - The ideas were further refined to meet the context of the assignment.

#### Entry (24/09/21) - Team
- New team member in group, Liyinqin Li. SJM now has a group size of 4.
- 'energy production by river flow with rainfall' was chosen as the first topic for prototyping.
  - We found data for energy production by hydro station, with the corresponding river flow data.
  - We could not find sufficient rain fall data over a long period of time for the locations of the hydro stations.  
- Changed our topic to our second choice 'energy production by riverflow with electricity cost' due to the above reason.

#### Entry (01/10/21) - Team
- Found the data sets for power production by hydro stations, river flow, and electricity cost.
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
- Convert excel file from web in R directly.

#### Entry (08/10/21) - Team
- Spent most of time collaborating with another group, sharing our projects.
- Attempted to fix github issues regarding merging repositories.
- Compared hydro stations and the river flows of the rivers they reside on.

#### Entry (08/10/21) - Sujung
- Remove unnecessary data and organize the necessary data for comparing with other data.

#### Entry (10/10/21) - Jensen
- Identified the coordinates of each appropriate hydro station and created a tibble containing this data.

#### Entry (13/10/21) - Matt
- Used Jensens hydro station data to figure out which rivers/lakes they are on and for each, what data i can find on the aquarius portal.
- imported datasets into r, found issues with some, will resolve

#### Entry (15/10/21) - Richard
- Beginning write the report about this project.

#### Entry (15/10/21) - Team
- After comparing the river flow data with the hydro station fleet location information, we found the greatest level of accuracy to be by month. This presented us with only 11 data point for each hydro station, as the river flow data for April was missing aswell. For this reason, we have decided to extend the range of our data to multiple years.
- Furthermore, only 11 out of the 47 hydro stations identified contained useable river flow data from the source used.

#### Entry (15/10/21) - Matt
- Figured out i need to use monthly interval for some datasets, and all records for others, all data has 1 entry per month per data set.

#### Entry (22/10/21) - Matt
- Have made a few changes over the past days to my river notebook, nearly ready for combination with jensen's data, need to remove part of time rows.
- Have with the help of Thomas Li, developed a function to extract south island names from wikipedia, which will be used with Sujungs data to obtain south island electricity costs.

#### Entry (22/10/21) - Team
- finalising data, almost ready to start combining and then graph some data, starting work on presentation.

#### Entry (22/10/21) - Richard
- Beginning write the power point for the presentation.

#### Entry (22/10/21) - Jensen
- Finished the automated scraping for the chosen range of years to get the data for (2015 to 2020)

#### Entry (23/10/21) - Sujung
- Converted numeric to date. But he first column name disappeared and the dates were converted. I will solve this problem with Richard and combine it with other data.

#### Entry (23/10/21) - Jensen
- Using map or lapply is really slow when applying functions to a list of tibbles. Instead I have used the 'furrr' package which allows for parallelization of the the purr functions.
- Using Matt's river flow data I tried to link the hydro stations power output with their corresponding rivers directly by name. However, this resulted in only one match, meaning I will have to manually search online to identify the code of the hydro stations that correspond to each river. For example, the hydro station in Raikaia is coded 'highbank', where as the hydro station in waitaki is also coded as 'waitaki'.
- Manual searching involves identifying the owner of the hydro stations situated on each river through the generation fleet spreadsheet extracted, then viewing the website of that company to identify its alternate name.
- I have identified the corresponding power station for each river, where available.
- I have converted Matt's river data so that the columns contain the correct data type. Using this data, I have combined it with the generation output of the hydrostations

#### Entry(25/10/21) - Jensen
- Converted electricity cost data into a tidy format, which was then merged with the generation output of dataframe, and plotted

#### Entry(30/10/21) - Jensen
- Commented my side of the code and produced a plotting function to allow graphing by the specified town.

#### Entry(30/10/21) - Matt
- Commented my side of the code

#### Entry(01/10/21) - Team
- Just finishing the report now
