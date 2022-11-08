# Microsoft on the Big Screen


![photo of people at the movies](https://github.com/emmigalfo/dsc-phase-1-project-v2-4/blob/master/Images/in_the_theatre.jpeg)

**Author:** [Emmi Galfo](mailto:emmi.galfo@gmail.com)


## Overview 


This project aims to guide Microsoft as it gets into the movie industry. Through exploratory analysis, factors such as genre, directors, movie runtime, and production budget are analysed to determine effects on net profit and return on investment. It turns out that what is needed for a higher return on investment is different than what is needed for a higher net profit. Higher budget films in the animation, kids & family, and fiction & fantasy genres make more net profit, whereas lower budget films in the horror, special interest, and documentary genres have higher returns on investment. 

## Business Problem

Microsoft is looking to get into the movie industry by starting their own movie studio. They need someone to explore what makes movies successful and provide them with reccommendations. For a business, being profitable is one great way to measure success. This project looks at the following variables and their potential to affect Microsoft's return on investment as well as their net profit:
*  Genre
*  Director
*  Runtime
*  Production Budget

## Data Understanding

In order to see which movies are most successful and why, reliable data is needed! Fortunately, there are plenty of excellent websites which gather all sorts of information on movies. All of the exploratory analysis for this project was able to be done with just two main data sets. 
* First, a data set was collected from the website, The Numbers, which supplies movies budgets and worldwide gross figures. 
* Second, a data set from Rotten Tomatoes was used to get information about movies' genres, directors, and runtime. 
* The two data sets were then joined together to analyse. 

## Data Analysis

#### Before we start...
Let's get an idea of what the data set shows by asking the following questions:
 1. What are the average and median ROI's and net profit?
 2. Which movies had the highest ROI's? 
 3. Which movies had the highest net profit? 

This will help us get a baseline knowledge of what is "normal" for the industry.

Analysis Shows:
* Average net profit: $59 Million USD
* Median net profit: $8.5 Million USD
* Min net profit: $-200 Million USD
     * Movie: Dark Phoenix
* Max net profit: $2.351 Billion USD
     * Movie: Avatar
* Net profit range: $2551 Million USD
* Average ROI: 3.8
* Median ROI: 0.7
* Min ROI: -1.0
   * Movie: Hayride
* Max ROI: 1799.0
   * Movie: Deep Throat
* ROI range: 1800.0

*Great news for Microsoft! Although there is a huge span when it comes to net profit, the median is around 8.5 million! Looking at what they can expect for a return on investment, there is once again a giagantic range with the min being -1 and a low budget movie bringing a max ROI of 1799! Here again, great news, while most movies do not have an ROI anywhere close to 1799, the median is still positive around 0.7.*  


### Factor 1: Production Budget
***

__Question__: Does it take money to make money?
![Scatterplot of production budget vs net profit](https://github.com/emmigalfo/dsc-phase-1-project-v2-4/blob/master/Images/Budget_NP.png)
__Answer__: In the movie industry the trend says yes!

__Question__: For a high net profit how much should be spent on production?

__Answer__: Taking the top 100 movies in terms of net-profit and looking at the median production budget and net profit, we see that Microsoft can expect to spend around 160 million to produce a movie that earns someplace in the ball park of 780 million USD!

__Question__: What kind of budget will see the most return on investment?
![Scatterplot of production budget vs ROI](https://github.com/emmigalfo/dsc-phase-1-project-v2-4/blob/master/Images/Budget_ROI.png)
__Answer__: It seems that for a higher return on investment, lower budget films are where its at.

*However, while this is good information to have, based on our previous finding that it takes money to make money, I think that Microsoft will be better off putting more money in for a higher net profit.*

__Question__: For a high return on investment how much should be spent on production?

__Answer__: Taking the top 100 movies in terms of return on investment and looking at the median production budget and return on investment, Microsoft can expect to spend around 7 million for a return on investment that is close to 5900%!


### Factor 2: Runtime
***
__Question__: How long should a movie's runtime be to make the most net profit?
![Scatterplot of runtime vs net profit](https://github.com/emmigalfo/dsc-phase-1-project-v2-4/blob/master/Images/Runtime_NP.png)
__Answer__: Try to stay within 80 minutes to 140 minutes to produce the most net profit.

__Question__: How long should a movie's runtime be to make the most return on investment?
![Scatterplot of runtime vs ROI](https://github.com/emmigalfo/dsc-phase-1-project-v2-4/blob/master/Images/Runtime_ROI.png)
__Answer__: Somewhere around 100 minutes in length brings the most ROI. 

### Factor 3: Directors
***

__Question__: Which directors bring in the most net profit, and what is the average production budget for their movies?
![Barplot of directors vs net profit](https://github.com/emmigalfo/dsc-phase-1-project-v2-4/blob/master/Images/Director_NP.png)
__Answer__: 
- Jean Negulesco (deceased)
1. Jennifer Lee 
2. Kyle Balda
3. James Cameron

*Average production budget for the top ten directors: 117 million USD*


__Question__: Which directors bring the highest return on investment, and what is the average production budget for their movies?
![Barplot of directors vs return on investment](https://github.com/emmigalfo/dsc-phase-1-project-v2-4/blob/master/Images/Director_ROI.png)
__Answer__: 
1. Oren Peli
2. Eduardo Sánchez
3. Daniel Myrick

*Average production budget for the top ten directors: 820 thousand USD*

### Factor 4: Genre
***
__Question__: Which genres average the highest net profit?
![Barplot of Genre vs net profit](https://github.com/emmigalfo/dsc-phase-1-project-v2-4/blob/master/Images/Genre_NP.png)
__Answer__: 
1. Animation
2. Kids & Family
3. Fiction & Fantasy

__Question__: Which genres average the highest ROI?
![Barplot of Genre vs ROI](https://github.com/emmigalfo/dsc-phase-1-project-v2-4/blob/master/Images/Genre_ROI.png)
__Answer__:
*While cult classics have the highest ROI, how to cause a movie to become a cult classic is beyond the scope of this project. Therefore, cult movies will not be listed in our top 3.* 
1. Horror
2. Special Interest
3. Documentary

## Evaluation

1. In the movie industry, it takes money to make money. Microsoft should be going for a larger net profit instead of a higher return on investment with a much lower net profit.
 2. For Microsoft to make the most net profit they should:
    * put more money into their production budgets (117-160 million USD)
    * hire directors Jennifer Lee, Kyle Balda, and James Cameron
    * make movies within genres Animation, Kids & Family, and Fiction & Fantasy
    * keep runtimes within 80 to 140 minutes
3. If Microsoft wants to make some lower budget movies (820,000-7 million USD), they can still get a high return on investment if they:
    * hire directors Oren Peli, Eduardo Sánchez, and Daniel Myrick
    * make movies within genres Horror, Special Interest, and Documentary
    * keep the runtimes around 100 minutes

## Conclusions

This project is a good starting place for Microsoft. However, due to time constraints, there are more factors that I would take into consideration before feeling confident about my reccomendations. Factors such standard deviation and inflation should be taken into consideration for future projects.
***
Thank you!

Emmi Galfo

emmi.galfo@gmail.com

