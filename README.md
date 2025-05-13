# ematm0061-lab-3-solved
**TO GET THIS SOLUTION VISIT:** [EMATM0061 Lab 3 Solved](https://www.ankitcodinghub.com/product/ematm0061-lab-3-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;93059&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;EMATM0061 Lab 3 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
This document describes your third assignment for Statistical Computing and Empirical Methods (Unit EMATM0061) on the MSc in Data Science. Before starting the assignment it is recommend that you first watch video lectures 6, 7 and 8.

You are encouraged to discuss these questions with your colleagues.

Begin by creating an Rmarkdown document with html output. You are not expected to hand in this piece of work, but it is a good idea to get used to using Rmarkdown.

Several optional extra questions have also been included. These are marked by stars (*). It is recommended that you first complete all unstarred questions before proceeding through the starred questions.

1 Random experiments, events and sample spaces

Our first question focuses on key concepts introduced in Lecture 7. Firstly, write down the definition of random experiment, event and sample space.

In small groups come up with your own probabilistic example:

• What is the random experiment in your example? • What are the possible outcomes in your example? • What are the events in your example?

• What is the sample space in your example?

2 Tidy data and iteration

We now return to the data wrangling concepts discussed in section 7.

2.1 Missing data and iteration

In this task we investigate the effect of missing data and imputation on plots. 1

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
The following function performs imputation by mean. What library do we need to load to run this function?

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
impute_by_mean&lt;-function(x){

mu&lt;-mean(x,na.rm=1) # first compute the mean of x

impute_f&lt;-function(z){ # coordinate-wise imputation if(is.na(z)){

return(mu) # if z is na replace with mean }else{

return(z) # otherwise leave in place }

}

return(map_dbl(x,impute_f)) # apply the map function to impute across vector }

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
Create a function called impute_by_median which imputes missing values based on the median of the sample, rather than the mean.

You can test your function on the following sample vector:

## [1] 1 2 2 4

Next generate a data frame with two variables x and y. For our first variable x we have a sequence (x1,x2,…,xn) where x1 = 0, xn = 10 and for each i = 1,…,n − 1, xi+1 = xi + 0.1. For our second variable y we set yi = 5 × xi + 1 for i = 1, . . . , n. Generate data of this form and place within a data frame called df_xy.

<pre>df_xy%&gt;%head(5)
</pre>
<pre>##     x   y
## 1 0.0 1.0
## 2 0.1 1.5
## 3 0.2 2.0
## 4 0.3 2.5
## 5 0.4 3.0
</pre>
The map2() function is similar to the map() function but iterates over two variables in parallel rather than one. You can learn more here https://purrr.tidyverse.org/reference/map2.html. The following simple example shows you how map2_dbl() can be combined with the mutate() function.

## x y z

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>v&lt;-c(1,2,NA,4)
impute_by_median(v)
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>df_xy%&gt;%
  mutate(z=map2_dbl(x,y,~.x+.y))%&gt;%
  head(5)
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
<pre>## 1 0.0 1.0 1.0
## 2 0.1 1.5 1.6
## 3 0.2 2.0 2.2
## 4 0.3 2.5 2.8
## 5 0.4 3.0 3.4
</pre>
We will now use map2_dbl() to generate a new data frame with missing data.

First create a function sometimes_missing with two variables index and value. The function should return

NA if index is divisible by 5 and returns value otherwise. Your function should produce the following outputs: sometimes_missing(14,25)

## [1] 25

<pre>sometimes_missing(15,25)
</pre>
## [1] NA

Next generate a new data frame called df_xy_missing with two variables x and y, but some missing data. For the first variable x we have a sequence (x1 , · · · , xn ), which is precisely the same as with df_xy. For the second variable y we have a sequence (y ̃1,··· ,y ̃n) where y ̃i = NA if i is divisible by 5 and y ̃i = yi for i not divisible by 5. To generate the dataframe d_xy_missing you may want to make use of the functions row_number(), map2_dbl(), mutate() as well as sometimes_missing().

Check that the first ten rows of your data frame are as follows:

<pre>##      x   y
## 1  0.0 1.0
## 2  0.1 1.5
## 3  0.2 2.0
## 4  0.3 2.5
## 5  0.4  NA
## 6  0.5 3.5
## 7  0.6 4.0
## 8  0.7 4.5
## 9  0.8 5.0
## 10 0.9  NA
</pre>
Create a new data frame df_xy_imputed with two variables x and y. For the first variable x we have a sequence (x1 , · · · , xn ), which is precisely the same as with df_xy. For the second variable y we have a sequence (y1′ , · · · , yn′ ) which is formed from (y ̃1 , · · · , y ̃n ) by imputing any missing values with the median. To generate df_xy_imputed from “‘df_xy_missing by applying a combination of the functions mutate and impute_by_median().

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>df_xy_missing%&gt;%
  head(10)
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
3

</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="section">
<div class="layoutArea">
<div class="column">
## x y r0 r1 r2 ## 1 0.0 1.0 1 1 1 ## 2 0.1 1.5 2 2 1 ## 3 0.2 2.0 3 3 1 ## 4 0.3 2.5 4 4 1 ## 5 0.4 3.0 5 5 1 ## 6 0.5 3.5 6 6 1 ## 7 0.6 4.0 7 7 1 ## 8 0.7 4.5 8 8 1 ## 9 0.8 5.0 9 9 1 ##100.95.51010 1

Combine the dataframes df_xy, df_xy_missing and df_xy_impute within a single dataframe called df_combined, along with an additional column indicating the source of the data.

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
<pre>df_xy&lt;-df_xy%&gt;%
  mutate(source="original")
</pre>
<pre>df_xy_missing&lt;-df_xy_missing%&gt;%
  mutate(source="corrupted")
</pre>
<pre>df_xy_impute&lt;-df_xy_impute%&gt;%
  mutate(source="imputed")
</pre>
<pre>df_combined&lt;-rbind(df_xy,df_xy_missing,df_xy_impute)
</pre>
</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
Plot the original data, the corrupted data and the imputed data together together with a trend line for each sample.

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>ggplot(df_combined,aes(x=x,y=y,color=source))+geom_point()+
  facet_wrap(~source)+geom_smooth(method="lm")
</pre>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
corrupted

</div>
</div>
<div class="layoutArea">
<div class="column">
imputed

</div>
</div>
<div class="layoutArea">
<div class="column">
original

</div>
</div>
<div class="layoutArea">
<div class="column">
50

40

30

20

10

0

</div>
</div>
<div class="layoutArea">
<div class="column">
0.0 2.5 5.0 7.5 10.00.0 2.5 5.0 7.5 10.00.0 2.5 5.0 7.5 10.0

x

</div>
</div>
<div class="layoutArea">
<div class="column">
source corrupted

imputed original

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
Do the imputed values yi′ give reasonable estimates of the true values yi? 4

</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
y

</div>
</div>
</div>
</div>
<div class="page" title="Page 5">
<div class="layoutArea">
<div class="column">
2.2 Tidying data with pivot functions

In this task you will read in data from a spreadsheet and apply some data wrangling tasks to tidy that data.

First download the excel spreadsheet entitled “HockeyLeague.xlsx”. The excel file contains two spread- sheets – one with the wins for each team and one with the losses for each team. To read this spreadsheet into R we shall make use of the readxl library. You may need to install the library:

<pre>install.packages("readxl")
</pre>
The following code shows how to read in a sheet within an excel file as a data frame. You will need to edit the folder_path variable to be the directory which contains your copy of the spreadsheet.

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
library(readxl) # load the readxl library folder_path&lt;-“your_folder_path…” # set this to the name of the

# directory containing “HockeyLeague.xlsx” file_name&lt;-“HockeyLeague.xlsx” # set the file name

file_path&lt;-paste(folder_path,file_name,sep=””) # create the file_path wins_data_frame&lt;-read_excel(file_path,sheet=”Wins”) # read of a sheet from an xl file

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
Inspect the first 3 rows of the first five columns:

<pre>## # A tibble: 3 x 5
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>wins_data_frame %&gt;%
  select(1:5)%&gt;%
  head(3)
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
## …1

## &lt;chr&gt;

##1Ducks

## 2 Eagles 24 of 50 12 of 50 37 of 50 14 of 50 ##3Hawks 20of5022of5033of5011of50

</div>
</div>
<div class="layoutArea">
<div class="column">
‘1990‘ ‘1991‘ ‘1992‘ ‘1993‘ &lt;chr&gt; &lt;chr&gt; &lt;chr&gt; &lt;chr&gt; 30of5011of5030of5012of50

</div>
</div>
<div class="layoutArea">
<div class="column">
A cell value of the form “a of b” means that a games were won out of a total of b for that season. For example, the element for the “Ducks” row of the “1990” column is “30 of 50” meaning that 30 out of 50 games were won that season.

Is this tidy data?

Now apply your data wrangling skills to transform the “wins_data_frame” data frame object into a data frame called “wins_tidy” which contains the same information but has just four columns entitled “Team”, “Year”, “Wins”, “Total”. The “Team” column should contain the team name, the “Year” column should contain the year, the “Wins” column should contain the number of wins for that season and the “Total” column the total number of games for that season. The first column should be of character type and the remaining columns should be of integer type. You can do this by combining the following functions: rename(), pivot_longer(), mutate() and separate().

You can check the shape of your data frame and the first five rows as follows: 5

</div>
</div>
</div>
<div class="page" title="Page 6">
<div class="layoutArea">
<div class="column">
wins_tidy%&gt;% dim() # check the dimensions

## [1] 248 4

wins_tidy%&gt;%head(5) # inspect the top 5 rows

<pre>## # A tibble: 5 x 4
##   Team   Year  Wins Total
##   &lt;chr&gt; &lt;int&gt; &lt;int&gt; &lt;int&gt;
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>## 1 Ducks  1990
## 2 Ducks  1991
## 3 Ducks  1992
## 4 Ducks  1993
## 5 Ducks  1994
</pre>
</div>
<div class="column">
<pre>30    50
11    50
30    50
12    50
24    50
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
The “HockeyLeague.xlsx” also contains a sheet with the losses for each team by season. Apply a similar procedure to read the data from this sheet and transform that data into a dataframe called “losses_tidy” with four columns: “Team”, “Year”, “Losses”, “Total” which are similar to thos in the “wins_tidy” data frame except for the “Losses” column gives the number of losses for a given season and team, rather than the number of losses.

You may notice that the number of wins plus the number of losses for a given team, in a given year does not add up to the total. This is because some of the games are neither wins nor losses but draws. That is, for a given year the number of draws is equal to the total number of games minus the sum of the wins and losses.

Now combine your two data frames, “wins_tidy” and “losses_tidy”, into a single data frame entitled “hockey_df” which has 248 rows and 9 columns: A “Team” column which gives the name of the team as a character, the “Year” column which gives the season year, the “Wins” column which gives the number of wins for that team in the given year, the “Losses” column which gives the number of losses for that team in the given year and the “Draws” column which gives the number of draws for that team in the given year, the “Wins_rt” which gives the wins as a proportion of the total number of games (ie. Wins/Total) and similarly the “Losses_rt” and the “Draws_rt” which gives the losses and draws as a proportion of the total, respectively. To do this you can make use of the mutate() function. You may also want to utilise the across() function for a slightly neater solution.

<pre>## Joining, by = c("Team", "Year", "Total")
</pre>
The top five rows of your data frame should look as follows:

<pre>hockey_df%&gt;% head(5)
</pre>
<pre>## # A tibble: 5 x 9
##   Team   Year  Wins Total Losses Draws Wins_rt Losses_rt Draws_rt
##   &lt;chr&gt; &lt;int&gt; &lt;int&gt; &lt;int&gt;  &lt;int&gt; &lt;int&gt;   &lt;dbl&gt;     &lt;dbl&gt;    &lt;dbl&gt;
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>## 1 Ducks  1990
## 2 Ducks  1991
## 3 Ducks  1992
## 4 Ducks  1993
## 5 Ducks  1994
</pre>
</div>
<div class="column">
<pre>30    50
11    50
30    50
12    50
24    50
</pre>
</div>
<div class="column">
<pre>20     0    0.6
37     2    0.22
</pre>
<pre> 1    19    0.6
30     8    0.24
 7    19    0.48
</pre>
</div>
<div class="column">
<pre>0.4      0
0.74     0.04
0.02     0.38
0.6      0.16
0.14     0.38
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
6

</div>
</div>
</div>
<div class="page" title="Page 7">
<div class="layoutArea">
<div class="column">
To conclude this task generate a summary data frame which displays, for each team, the median win rate, the mean win rate, the median loss rate, the mean loss rate, the median draw rate and the mean draw rate. The number of rows in your summary should equal the number of teams. These should be sorted in descending order or median win rate. You may want to make use of the following functions: select(), group_by(), across(), arrange().

2.3 Most correlated variables (*)

This data wrangling task is slightly more challenging. You may want to return to this task once you have completed the unstarred questions in sections 3 and 4 below.

The objective is to investigate, for each numerical variable within a data set, which other numerical variables have the largest correlation (in absolute value).

In lecture 6 we introduced the following function called “max_cor_var”. The function entitled “max_cor_var” takes as input a data frame “df” and a column name “col_name”. It then extracts the variable with name col_name and determines which other numerical variables within the data set have the highest correlation (in absolute value) with that variable. It then returns a data frame containing the name of the variable “var_name” and the corresponding correlation “cor”. Begin by making sure you understand the structure of the function.

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
max_cor_var&lt;-function(df,col_name){

# function to determine the variable with maximal correlation

v_col&lt;-df%&gt;%select(all_of(col_name)) # extract variable based on col_name

<pre>  df_num&lt;-df%&gt;%
    select_if(is.numeric)%&gt;%
    select(-all_of(col_name))
</pre>
<pre>  # select all numeric variables excluding col_name
</pre>
correlations&lt;-unlist(map(df_num, function(x){cor(x,v_col,use=”complete.obs”)}))

<pre>  # compute correlations with all other numeric variables
</pre>
max_abs_cor_var&lt;-names(which(abs(correlations)==max(abs(correlations)))) # extract the variable name cor&lt;-as.double(correlations[max_abs_cor_var])

# compute the correlation

<pre>  return(data.frame(var_name=max_abs_cor_var,cor=cor))
</pre>
<pre>  # return dataframe
</pre>
}

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
Next generate a new function called “top_correlates_by_var” which takes input a data frame “df” and outputs a data frame with a single row. The column names of this output data frame should coincide with the names of the numerical columns within the input dataframe “df”. For each column name, the value should be equal to variable name corresponding to the numerical variable which has the highest level of correlation (in absolute value) to the variable with that column name, but is not equal to it.

You can test your function as follows. By using the Palmer penguins data set you should obtain the following output.

</div>
</div>
<div class="layoutArea">
<div class="column">
7

</div>
</div>
</div>
<div class="page" title="Page 8">
<div class="section">
<div class="layoutArea">
<div class="column">
<pre>library(palmerpenguins)
</pre>
<pre>penguins%&gt;%
  top_correlates_by_var()
</pre>
</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>## # A tibble: 1 x 5
</pre>
<ul>
<li>
<pre>## &nbsp;  bill_length_mm    bill_depth_mm     flipper_length_mm body_mass_g   year
</pre>
</li>
<li>
<pre>## &nbsp;  &lt;chr&gt;             &lt;chr&gt;             &lt;chr&gt;             &lt;chr&gt;         &lt;chr&gt;
## 1 flipper_length_mm flipper_length_mm body_mass_g       flipper_leng~ flipper_l~
</pre>
Next use a combination of the functions group_by(), nest(), mutate(), select(), unnest() together with your new function top_correlates_by_var() to determine those variables with highest correlation, broken down by species of penguin. Your results should be as follows.

<pre>## # A tibble: 3 x 5
## # Groups:   species [3]
##   species   bill_length_mm bill_depth_mm  flipper_length_mm body_mass_g
</pre>
</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>##   &lt;fct&gt;
## 1 Adelie
## 2 Gentoo
## 3 Chinstrap bill_depth_mm  bill_length_mm body_mass_g
</pre>
3 Elementary set theory

In this section we consider some of the concepts introduced in Lecture 7.

</div>
<div class="column">
<pre>&lt;chr&gt;
bill_depth_mm
bill_depth_mm
flipper_length_mm
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>&lt;chr&gt;
body_mass_g
body_mass_g
</pre>
</div>
<div class="column">
<pre>&lt;chr&gt;
body_mass_g
body_mass_g
</pre>
</div>
<div class="column">
<pre>&lt;chr&gt;
body_mass_g
bill_depth_mm
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
Remember that a set is just a collection of objects. All that matters for the identity of a set is the objects it contains. In particular, the elements within the set are unordered, so for example the set {1, 2, 3} is exactly the same as the set {3, 2, 1}. In addition, since sets are just collections of objects, each object can only be either included or excluded and multiplicities do not change the nature of the set. In particular, the set {1,2,2,2,3,3} is exactly the same as the set A = {1,2,3}. In general there is no concept of “position” within a set, unlike a vector or matrix.

3.1 Rolling a dice

Let’s suppose we role a dice. The set of possible outcomes is Ω := {1, 2, 3, 4, 5, 6} corresponding to the different sides of the dice which could land face up.

Let’s introduce events A, B defined by A := {1,2,3}, B := {2,4,6}, C := {4,5,6}. Unions

What is A∪B?

What is A∪C?

Intersections

What is A∩B?

</div>
</div>
<div class="layoutArea">
<div class="column">
8

</div>
</div>
</div>
<div class="page" title="Page 9">
<div class="layoutArea">
<div class="column">
What is A∩C?

Complements

What is A\B? What is A\C?

Disjointness

Are A and B disjoint?

Are A and C disjoint?

Partitions

Write down a partition of Ω := {1, 2, 3, 4, 5, 6} consisting of two sets. Write down another partition of Ω containing three sets.

3.2 Complements, subsets and De Morgan’s laws

LetΩbeasamplespace. RecallthatforaneventA⊆ΩthecomplementAc ≡Ω\A:={ω∈Ω : ω∈/A}. Take a pair of events A ⊆ Ω and B ⊆ Ω.

</div>
</div>
<div class="layoutArea">
<div class="column">
Complements

Can you give an expression for (Ac)c without using the notion of a complement? What is Ωc?

Subsets

Show that if A ⊆ B then Bc ⊆ Ac.

</div>
</div>
<div class="layoutArea">
<div class="column">
Intersections

</div>
</div>
<div class="layoutArea">
<div class="column">
Show that (A ∩ B)c = Ac ∪ Bc.

Let’s suppose we have a sequence of events

</div>
<div class="column">
⊆ Ω.

⊆ Ω.

</div>
</div>
<div class="layoutArea">
<div class="column">
􏰃􏰡K

k=1 Ak

Union

</div>
<div class="column">
􏰄c

</div>
<div class="column">
A1, A2, . . . , AK in terms of unions and complements?

</div>
<div class="column">
Can you

Can you

</div>
<div class="column">
write

write

</div>
<div class="column">
out an

out an

</div>
<div class="column">
expression for

expression for

</div>
</div>
<div class="layoutArea">
<div class="column">
Show that (A ∪ B)c = Ac ∩ Bc.

Let’s suppose we have a sequence of events A1, A2, . . . , AK

</div>
</div>
<div class="layoutArea">
<div class="column">
􏰃􏰠K

k=1 Ak

</div>
<div class="column">
􏰄c

in terms of intersections and complements?

</div>
</div>
<div class="layoutArea">
<div class="column">
Note The results (A ∩ B)c = Ac ∪ Bc and (A ∪ B)c = Ac ∩ Bc are often referred to as “De Morgan’s laws”. 3.3 Cardinality and the set of all subsets

Suppose that Ω = {ω1,ω2,…,ΩK} contains K elements for some natural number K ∈ N. Hence, Ω has cardinality K.

</div>
</div>
<div class="layoutArea">
<div class="column">
9

</div>
</div>
</div>
<div class="page" title="Page 10">
<div class="layoutArea">
<div class="column">
Let E := {A ⊆ Ω} be the set of all subsets. Give a formula for the cardinality of E in terms of K.

3.4 Disjointness and partitions

Suppose we have a sample space Ω.

Can you think of a set which is disjoint from every other set? That is, find a set A ⊆ Ω such that A∩B = ∅

for all sets B ⊆ Ω.

Suppose we have events A1, A2, A3, A4 all subsets of Ω.

DefineeventsS1,S2,S3,S4 allsubsetsofΩbyS1 :=A1,S2 :=A2\A1,S3 :=A3\(A1∪A2),S4 := A4 \(A1 ∪A2 ∪A3).

Show that S1, S2, S3, S4 form a partition of A1 ∪A2 ∪A3 ∪A4. 3.5 Uncountable infinities (**)

This is a challenging optional extra. You may want to return to this question once you have completed section 4.

Show that the set of numbers Ω := [0, 1] is uncountably infinite.

4 Introduction to probability

In this section we consider some of the concepts introduced in Lecture 8.

4.1 Probability of a complement

Prove that if Ω is a sample space, S ⊆ Ω is an event and Sc ≡ Ω \ S is its complement we have P(Sc) = 1 − P(S).

4.2 The union bound

The third rule of probability states that if we a sequence of disjoint sets A1 , A2 , A3 , . . . then

􏰚∞􏰛∞

P 􏰢Ak =􏰁P(Ak).

k=1 k=1

We also no from the union bound that for any sequence of sets A1, A2, A3, . . . whatsoever (not necessarily

</div>
</div>
<div class="layoutArea">
<div class="column">
disjoint) we have

</div>
</div>
<div class="layoutArea">
<div class="column">
􏰚∞􏰛∞

P 􏰢Ak ≤􏰁P(Ak).

k=1 k=1

</div>
</div>
<div class="layoutArea">
<div class="column">
Give an example sequence of sets A1, A2, A3, . . . in which P (􏰠∞k=1 Ak) ̸= 􏰖∞k=1 P(Ak). 10

</div>
</div>
</div>
<div class="page" title="Page 11">
<div class="layoutArea">
<div class="column">
4.3 Verifying the rules of probability

Consider a setting in which Ω = {0, 1}, and E := {∅, {0}, {1}, {0, 1}}. Fix q ∈ [0,1] and define a probability P : E → [0,1] by

0 if A = ∅ 1−q ifA={0} q if A = {1} 1 if A = {0, 1}.

Verify that the probability space (Ω,E,P) satisfies the three rules of probability. 4.4 Rotation invariant measures on [0,1] (***)

This is a challenging optional extra.

I recommend completing the other questions on the assignment first.

Consider the sample space Ω := [0, 1). Recall that for a real number x ∈ R, the floor ⌊x⌋ denotes the largest integer n ∈ Z with n ≤ x. Given a number a ∈ R we define a rotation map Ta : Ω → Ω by

Ta(x) := (x+a)−⌊(x+a)⌋. Observe that Ta : [0, 1] → [0, 1] is a one-to-one mapping.

A probability P on Ω is said to be rotation invariant if for any event A ∈ E and any a ∈ R we have P[Ta(A)] = P(A).

Show that we cannot define a rotation invariant probability measure on E := {A ⊆ Ω}, the set of all sets. This means that we must restrict such probability measures to a “well-behaved” σ-algebra!

If you have completed all the questions on this assignment email henry.reeve@bristol.ac.uk.

</div>
</div>
<div class="layoutArea">
<div class="column">
P(A) :=

</div>
</div>
<div class="layoutArea">
<div class="column">
11

</div>
</div>
</div>
