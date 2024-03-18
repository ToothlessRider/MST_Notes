#  DM Notes for MST
> Author : Aaron Augustine

> Star the gist so that I can get a consensus on how many people are using this resource


## PYQ's
#### 0.1 a. Fill in the blanks
1.  Name the characteristic of the data where presence counts.
2. Converting data from different sources into a common format for processing is called as ______
3. Assume you want to perform supervised learning and to predict the height of a lace above the sea level, it is an example of ________

*Ans*. 
1. Categorical Data
2.  Data Integration
3. Regression


<hr>

#### Q1 b. Differentiate between
a) Knowledge discovery and data mining
b) Nominal and ordinal Attributes
c) OLAPand OLTP

*Ans*


#### Q1 C. Suppose that our goal is to calculate the similarity of the two documents given below.
>Document I = 'the best data science course'
Document 2 = 'data science is popular'
Compute the similarity using cosine and jaquards' measures

*Ans*


<hr> 

#### Q2 a.The dataset below contains categorical descriptions of samples corresponding to 10 samples of grilled mushroom. Each mushroom is classified as poisonous?={yes,no}
**![](https://lh7-us.googleusercontent.com/n0QO0jrvUYFM2sd6np-vV1BTX_Z4vYf-MYRoooA5x1ttlMSYPJJvJWBV4t3J1AMsWFwoRHe2-NK4pMiFfG7qFXrYX53V4_4dTw0OpPkyEQXssmTrGLgVzPc-AISU7upNdippl5mOA18kOUylmLTcXqg)**
* Construct the contingency table of conditional an prior class probabilities  that would be used by Naive Bayes classifier to build the classifier for the dataset above.
* Based on the contingency table, use Naive Bayes to estimate the likelihood
that the following mushroom is poisonous. Show your calculations.

*Ans* 


<hr>

#### Q2 b.Given four objects represented by the tuples (28, 5, 46, 15), (l5, 25, 3, 12). Compute the Euclidean, Manhattan, Minkowski (p=3) distance between the objects.
*Ans*


<hr>

#### Q3 a. Suppose that the data for analysis includes the attribute age. The age values for the data tuples are (in increasing order) : 12, 26, 69, 72.
* Use min-max normalization to transform the values for age onto the
range [0. I]
* Use Z-Score normalization to transform the values for age

*Ans*

<hr>

#### Q3 b.The confusion matrix below summarizes the perfo ances of a binary classifier applied to dataset of an example labels  which are annoted by two labels ( Yes, No )
|--| Yes|No|
|--|--|--|
|Yes|32|46|
|No|65|122|

Based on the matrix, calculate : 
	a) F score 
	b) Accuracy 
	c) Precision 
	d) Recall

*Ans*

<hr>

#### Q4 a. Define data integration. Why is it needed? Discuss the various issues associated with data integration

*Ans*

<hr>

#### Q4 b.Explain the major tasks in data preprocessing

*Ans*

<hr>

## Exam Questions

**Q1. What is Data Mining ? Give some  uses of data mining and examples of data mining applications **
*Ans* 
* It is the efficient discovery of previous *unknown*, *potentially useful* patterns within large datasets
* The analysis of observational datasets to find unsuspected relationships and to summarize the data in new ways, that are understandable and useful.

**General Terms** : 
* *Data* : A set of __facts__ stored in a database.
* *Pattern* : An discernible regularity or trend that __describes a subset of facts__
* *Attribute* : A __characteristic feature of a data object__ within data 
* *Interestingness* :  The **degree** to which a **discovered pattern** or association in data is **considered valuable**.

Data mining is used for the following purposes : 
1. To *Identifty the problem*
2. To *transform* data into *information*
3. Act on information
4. Measure the results


 
**Applications of DM** : 
* Fraud Detection
* Marketing
* Data warehousing
* Astronomy
* Molecular Biology


<hr>

The Process of knowledge discovery in data mining follows the given set of steps :

**![](https://lh7-us.googleusercontent.com/1PeOBbWmnK-eLkeRZj2eBh3Sn2UHFd3af9Orgrv26plnQ8XZlu72C2qtP3R282c_ftzcPyFLkxZ3k_JuENOiZRmWI04AhFqIpth2BPknE-0BgJCRL_1zoRMzStBJ-3a7zv6h2btzzcERgtP2Csispio)**

<hr>

**Q2.   What are the different data mining tasks?**
*Ans*. The difference data mining tasks are as follow : 
* __Classification __: Leaning a function that maps an item into a set of predefined classes.
* __Regression__ : Learning a function that maps an item to a real value.
* __Clustering__ : Identify a set of groups of similar items .
* __Dependency and Associations__ : Identify any *significant dependencies* between data *attributes*.
* __Summarization__ : 
