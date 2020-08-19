# Modeling-NBA-Games using Data and Bivariate Hawkes Processes
## Research conducted alongside Professor J. Pender, Operations Research and Information Engineering, Cornell University
NBA Basketball is arguably the most exciting sport in the world. With quite an abundance of actively invested NBA fans—producing data-driven models and simulations of live games would prove to be very beneficial. We gather play-by-play data from the 2018-2019 NBA season to not only develop shooting patterns and playing trends for all 30 teams but to also analyze the inter-arrival times of shots taken and made in a game. We use the results from this data to understand team preferences for shooting two- and three-pointers and finally, model each NBA game as a bivariate Hawkes process. A Hawkes process is a self–exciting model in which the occurrence of an event increases the probability of another event occurring. Ultimately, this model supposes that past events can temporarily raise the probability of future events. Bivariate Hawkes processes—a variation of Hawkes process—is relevant for the NBA because when one team scores in basketball, the other team obtains the ball and it increases the likelihood that the other team scores during the next possession. Thus, the back and forth dynamic of a basketball match lends itself naturally to bivariate Hawkes models.

# Methods:
i. Imported 2018-2019 NBA play-by-play data and used Python data science packages (numpy, pandas, matplotlib, seaborn, plotpy, etc) to thoroughly parse, clean and organize the data by home/away team, game type, shot type and several other categories needed to calculate the parameters for a bivariate Hawkes model

ii. Once data has been gathered, we devised a series of short algorithms to compile team shooting preferences and calculate the inter-arrival times between each shot taken and made for each shooting category (free throws, two-pointers, three-pointers, etc.). Before proceeding to pass these findings into our Hawkes model, we added visual representations of this data to evaluate its accuracy. (Refer to Figures 1 and 2 from research poster)

iii. After compiling the shooting trends for each shot category, inter-arrival times, and all necessary numerical calculations and percentages relevant for replicating an NBA game, we proceeded to use these findings as parameters for our bivariate Hawkes model. In theory, an ideal model would accurately reflect the progression of any NBA game from quarters 1-4 (and any overtime sessions thereafter) so we refined the model’s parameters until it nearly reflected this desirable outcome. Without using a bivariate Hawkes process, it would have been severely difficult to accurately depict the probable scoring of a team, for this scoring is directly affected by the events that occur in the previous team’s possession.
