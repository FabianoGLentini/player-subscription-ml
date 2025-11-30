
# Q1 From planning phase: 
Which player characteristics and behaviours best predict subscription to a game-related newsletter, and how do these differ among player types?

## Our Question: 
What players' `Age`, `gender`, and `played_hours` can best predict whether they would `subscribe` to a gaming newsletter, and how does it differ from players `experience`?



## Project Report Breakdown 

> [Tip & Info]
>
> Check out Individual Planning. We can use our proposals to pull out completed tasks or descriptions and polish them to speed up the process and avoid duplicating work that we have already done.
>
>  **Teams Individual Planning Links**
>
>  Result was `Good` for both `Mechanics` and `Reasoning.`
>
>  Link:  https://github.com/FabianoGLentini/DSCI_100_Planning 
>  (Heads up, I believe I lost marks for using too many graphs without a clear reasoning behind them.)

> [Key Point To Make / Important to note across project]
> - This is a **Classification** problem
> - We are using `Age`, `gender`, and `played_hours` as our **Predictors**
> - We are looking for resulting **binary outcome** of `subcription`
> - We are using **K-nearest neighbors model** for our Classification question
> - We are using **cross-validation to choose k**
> - We are using a **confusion matrix** to evaluate the performance of our result. 
> 	- We are using **Accuracy** to determine, overall, how well our model predicts our data using our test data
> 	- We will use **Recall**  (To check false negatives) and **Precision** (To check false positives)  to help us identify problems our models may have run into
> 	- Putting more emphasis on **Precision** to **reduce false positives** would better fit our goal to identify players who are most likely to subscribe. We are not as interested in players who would not subscribe, so we must get the most precise true subscription prediction.
>

## To-do's:

## Introduction: (Maeve) (Word Count: ~ 300-400)
    
- [ ] Provide some relevant background information on the topic so that someone unfamiliar with it will be prepared to understand the rest of your report
    
- [ ] Clearly state the question you tried to answer with your project
    
- [ ] Identify and fully describe the dataset that was used to answer the question **(Maybe explain why we chose the selected variables)**
    
---
## Methods & Results: (Split Maeve, Fabiano, Riley)  (Total Word Count: ~ 1000 - 1200)

> [Important]
>
>  Describe the methods you used to perform your analysis from beginning to end, which narrates the analysis code. 
>
>  All figures should have a figure number and a legend

### Set up and intro to data: (Maeve/Fabiano)  (Word Count: ~ 300-400)

- [x] Load data *(Fabiano)*
    
- [x] Wrangles and cleans the data to the format necessary for the planned analysis **(From Planning phase if appropriate)** *(Fabiano)*
    
- [ ] Performs a summary of the data set that is relevant for exploratory data analysis related to the planned analysis  **(From Planning phase if appropriate)**
    
- [ ] Creates a visualization of the dataset that is relevant for exploratory data analysis related to the planned analysis **(Histogram could be good?)**
- [ ] Add additional comment/analysis of perceived issues for our experiment **(From Planning phase if appropriate, "I am unsure if this is expected of us or not but its already been done so if we have room might as well include it")**
---
### Training and Analysis: (Fabiano)  (Word Count: ~ 400-500)

> [Important]
>
> Must use seed() for reproducibility.
>
> Include legends for each figure, reference book, or worksheet for a clearer idea of how to manage.
>
> Explain steps taken and why



- [ ] Performs the data analysis/training
	- [ ] Split/Scale/Encode
	- [ ] K-fold cross-validation to find k
	- [ ] Fit Models
		**Main models:**
		- [ ] Age + Gender + played_hours
		- [ ] Age + played_hours
		- [ ] Age + Gender
		- [ ] Gender + played_hours
		
		**Potential additional models if useful:**
		- [ ] Age
		- [ ] Gender
		- [ ] played_hours
		
    
- [ ] Creates a visualization of the analysis 
	- [ ] Confusion Metrics for model comparison Using Accuracy
		- [ ] Precision (**we value this more**)
		- [ ] Recall (**To see if any glaring issues**)
	- [ ] Additional visuals needed (scatterplot per model demonstrating result?)
- [ ] Comment on the results of confusion metrics and model performances
#### Player Types Exploration (Insight) (Riley)  (Word Count: ~ 200-300)

- [ ] Additional visual and graph for analysis **(Note we may not need all of these they are suggestions we mainly need to address "how does it differ from players `experience`?")**
	- [ ] Show subscription rate by experience level
	- [ ] Player_hour relates to experience
	- [ ] Age vs experience
- [ ] Commend/Analyze Results 
    
---
### Discussion: (Riley)  (Word Count: ~ 300-400)
    

- [ ] Summarize what you found
    
- [ ] Discuss whether this is what you expected to find **(Check Planning Faze I think there may be some info to reference there)**
    
- [ ] Discuss what impact such findings could have 
    
- [ ] Discuss what future questions this could lead to
    
    > [If Needed]
	>
    > You may include references if necessary, as long as they all have a consistent citation style.
    
---