Are sharks sexist?


I guess this is a question that everyone is wanting to know the answer for. 
The purpose of this project is to analyze the data of shark attacks and resolve this doubts once and for all.

To begin, I will present a summary of the data I am going to use so we understand the capabilities of this study and its results.

The data set contains around 3500 incidents that apparently involved these giant fishes. For each case, we managed to gather information about where in the world happened, the date, the time of the day, the sex of the victim, their age, the activities they were doing, 
if they survived, and a link to an article related to the case.

After looking at this data set and clean it. I wanted to see if there is an existing pattern on the behavior of the sharks in terms of choosing the victim. In this case, if the sex of the victim has any impact on the shark's behavior.

I listed four hypotheses to help me understand the patterns.

1. Shark's nationality affects how sexist they are.

2. There are spieces more sexist than others. 

3. Female victims have a higher likelihood to suffer a lethal attack, compared to male victims.
	
4. Sharks prefer young and fresh ladies rather than old. 

5. The amount of attacks depends on the activity that the victim is doing.


These hypothesis will drive my investigation and will lead us to understand if sharks are sexist or not, if there is a specific species that it's still stuck in the last century, if sharks are more sexist in an specific areas of the world, and if the sharks tend
to be more aggressive against women. 


Results:

Before jumping into calculations and plots. I needed to clean the data set. All the code that I used is in the ipynb called "clean", in the same repo.
To summ up, I removed all the columns and rows that didn't contain any data or very few. This way I managed to have a bit less number of cases but with full information each of them.
I looked for duplicated, but this dataset didn't have any. 
I also wanted to group the values of the columns that had many different inputs. As an example, insted of having: ' Swiming fast, swiming slow, swiming and having fun', I wanted to have one group called 'swiming'.xº