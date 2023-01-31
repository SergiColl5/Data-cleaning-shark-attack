# Are sharks sexist?


I guess this is a question that everyone is wanting to know the answer for. 
The purpose of this project is to analyze the data of shark attacks and resolve these doubts once and for all.

To begin, I will present a summary of the data I am going to use so we understand the capabilities of this study and its results.

The data set contains around 6300 incidents that apparently involved these giant fishes. For each case, we managed to gather information about where in the world happened, the date, the time of the day, the sex of the victim, their age, the activities they were doing, if they survived, and a link to an article related to the case.

After looking at this data set and clean it. I wanted to see if there is an existing pattern on the behavior of the sharks in terms of choosing the victim. In this case, if the sex of the victim has any impact on the shark's behavior.

I listed four hypotheses to help me understand the patterns.

### 1. Shark's nationality affects how sexist they are.

### 2. There are species more sexist than others. 

### 3. Female victims suffer a fatal attack more often than male.
	
### 4. Sharks prefer young ladies rather than old boys.

### 5. Depending on what activity girls do, it is more likely to receive a shark attack.


These hypotheses will drive my investigation and will lead us to understand if sharks are sexist or not, if there is a specific species that it's still stuck in the last century, if sharks are more sexist in an specific areas of the world, and if the sharks tend
to be more aggressive against women. 


Results:

Before jumping into calculations and plots. I needed to clean the data set. All the code that I used is in the ipynb called "clean", in the same repo.
To sum up, I removed all the columns and rows that didn't contain any data or very few. This way I managed to have a smaller number of cases but with full information each of them.
I looked for duplicated values, but this dataset didn't have any. 
I also wanted to group the values of the columns that had many different inputs. As an example, instead of having: ' Swiming fast, swiming slow, swiming and having fun', I wanted to have one group called 'swiming'. After doing the same process for a few columns, I managed to have more consistent data.
Once everything looked decent enough, I started preparing the plots for the different hypothesis.


 **1. Shark's nationality affects how sexist they are.**
 
To know the nationality and its relation with the sex of the victim. I needed to know how many women had an incident with a shark by country. Since it is not useful to have total volumes, I added an additional column with the percentage of female victims out of the total cases per country. I ended up creating a crosstab, grouping by country and having the totals per female, male, and the percentage of female victims. 

![alt text](https://github.com/SergiColl5/Data-cleaning-shark-attack/blob/main/images/country_sex.jpg?raw=true)

As can be seen, sharks from the Mediterranean area are more likely to go after women than sharks from other parts of the world. Be careful out there, ladies…

**2. There are species more sexist than others.**

Believe it or not, sharks around can influence the behavior to each other. Maybe. Let’s see.
In order to obtain this information, I needed to group the species and calculate the percentage of women they attacked and below we can see the results. 

![alt_text](https://github.com/SergiColl5/Data-cleaning-shark-attack/blob/main/images/hammerhead_shark.jpg?raw=true)
![alt_text](https://github.com/SergiColl5/Data-cleaning-shark-attack/blob/main/images/bull_shark.jpg?raw=true)
![alt_text](https://github.com/SergiColl5/Data-cleaning-shark-attack/blob/main/images/tiger_shark.jpg?raw=true)
![alt_text](https://github.com/SergiColl5/Data-cleaning-shark-attack/blob/main/images/white_shark.jpg?raw=true)
![alt_text](https://github.com/SergiColl5/Data-cleaning-shark-attack/blob/main/images/wobbegong_shark.jpg?raw=true)
![alt_text](https://github.com/SergiColl5/Data-cleaning-shark-attack/blob/main/images/species_not_confirmed.jpg?raw=true)

In the end, there is not any species way worse than the others. I guess they just attack whatever they see moving and splashing. Let’s move onto the third hypothesis.

**3. Female victims suffer a fatal attack more often than male.**

This time, I had to group by the sex of the victim and see what was the result of the attacks, whether they survived or not. Who do you think survive more often? Girls or boys?

![alt_text](https://github.com/SergiColl5/Data-cleaning-shark-attack/blob/main/images/F.jpg?raw=true)
![alt_text](https://github.com/SergiColl5/Data-cleaning-shark-attack/blob/main/images/M.jpg?raw=true)

The answer is pretty clear, girls know better in terms of handling weird situations with strangers approaching them. But what is it because they are older and more experimented than the boys that are attacked? Let’s check our fourth hypothesis.

**4. Sharks prefer young ladies rather than old boys.**

To know the answer more accurately, I split the results by species, to see if there was a pattern. And here it is.

![alt_text](https://github.com/SergiColl5/Data-cleaning-shark-attack/blob/main/images/species_age.jpg?raw=true)


Sharks tend to attack young ladies but older boys. Despite boys being older on average, girls manage to survive more often, maybe we should reconsider some things… Anyways, our last hypothesis it is related to the activity of the victims.


**5. Depending on what activity girls do, it is more likely to receive a shark attack.**

![alt_text](https://github.com/SergiColl5/Data-cleaning-shark-attack/blob/main/images/activity_female.jpg?raw=true)
![alt_text](https://github.com/SergiColl5/Data-cleaning-shark-attack/blob/main/images/activity_boys.png?raw=true)



And yes, out of all the attacks, the activity that seems to have more difference is swimming. Boys are attacked more or less the same no matter the activity. But when it comes to girls, sharks prefer to have them directly in the water, instead of smashing a boat or a surfboard to get their victims.

### In conclusion, we have seen that there are some differences when it comes to sex, mostly because the majority of the attacks happened to boys. But in terms of preferences between ages and activities, we see a bit of a pattern. Do you think sharks can recognize if they are attacking a girl or a boy?







The repo contains two files and one folder: 'Clean','Explore' and 'Images'.
Clean: Code written in python. With defined functions in order to get rid of blank columns and rows, duplicates, and useless data.
Explore: Code written in python. With defined functions and methods to calculate, group, display the results and save them as image.
Images: All the plots saved in one folder. 


