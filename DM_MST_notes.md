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

**Q1. What is Data Mining and why do we do it ? Give some  uses of data mining and examples of data mining applications **
*Ans* 
* It is the efficient discovery of *non-trivial*, *implicit*,*previously-unknown*, *potentially useful* patterns within large datasets
* The analysis of observational datasets to find unsuspected relationships and to summarize the data in new ways, that are understandable and useful.

We're doing data mining, because we have an abundance of data but we're starving for knowledge / information.
Sources : Businesses, science, society

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

**Q2.   What are the different data mining tasks? Note the difference data mining methods**
*Ans*. The difference data mining tasks are as follow : 
* __Classification__  : Leaning a function that maps an item into a set of predefined classes.
* __Regression__ : Learning a function that maps an item to a real value.
* __Clustering__ : Identify a set of groups of similar items .
* __Dependency and Associations__ : Identify any *significant dependencies* between data *attributes*.
* __Summarization__ : To find a compact decription of the dataset.

<hr>

**Q3. Why not traditional data analysis ?**
*Ans* The use of traditional data analysis techniques has been reduced for the following reasonss : 
* Tremendous amounts of data 
	* Algorithms must be scalable so as to handle tera-butes of data
* High dimensionality 
	* A singular micro array may have tens of thousands of dimensions
* HIgh complexity of data
* New and sophisticated applications

<hr>

**Q4. What is data preprocessing ?  **

*Ans*. 

<hr>

**Q5. On what kinds of applications can you do data mining ?**

*Ans* Database oriented data sets and applications
* Relational Databases. data warehouses, transactional databases

Advanced datasets and advanced applications : 
* Data streams and sensor data
* Time series data, temporal data and sequence data
* Structure data, graphs, social networks, etc
* Object-relational databases
* Legacy databases
* Multimedia databases
* Text Databases
* Audio Databases, etc
* WWW

<hr> 

**Q6. What are the different Data Mining Functionalities ?**

*Ans* There are 7 basic functionalities of Data Mining : 
* *Multidimensional Concept Description*: 
	* To describe whatever has multiple dimensions, i.e. to generalize, summarize and categorize data characteristics
	* Ex. Dry vs Wet regions
* *Frequent patterns, associations, correlations vs causality*.
* *Classification and prediction*
	* Construct models that decribe classes for future prediction
	* Predict unknown or missing values 
* Cluster analysis
	* Class label is unknown: Group data to form new classes, e.g., cluster houses to find distribution patterns 
	* Maximizing intra-class similarity & minimizing interclass similarity
* Outlier analysis
	* Outlier: Data object that does not comply with the general behavior of the data 
	* Noise or exception? Useful in fraud detection, rare events analysis
* Trend and evolution analysis
	* Trend and deviation: e.g., regression analysis
	* Sequential pattern mining: e.g., digital camera -Y large SD memory
	* Periodicity analysis
	* Similarity-based analysis
* Other pattern-directed or statistical analyses

<hr>

**Q7. What are the Major issues in Data Mining ? **

*Ans*. 
* Mining methodology
	* Mining different kinds of knowledge from diverse data types, e.g., bio, stream, Web
	* Performance: efficiency, effectiveness, and scalability
	* Pattern evaluation: the interestingness problem 
	* Incorporation of background knowledge
	* Handling noise and incomplete data
	* parallel, distributed and incremental mining methods
	* Integration of the discovered knowledge with existing one: knowledge fusion
* User interaction
	* Data mining query languages and ad-hoc mining
	* Expression and visualization of data mining results
	* Interactive mining of knowledge at multiple levels of abstraction
* Applications and social impacts
	* Domain-specific data mining & invisible data mining
	* Protection of data security, inegrity and privacy

<hr>
**![](https://lh7-us.googleusercontent.com/ZLJdJs_9qqU4ScCQy2hg9tdwrfOUz7QJOf7APUBgerKWm3mGnU0tDovzFlpeWZCx4YgMwk7AksLoVOOrOEo_jwnea-dTG-4Ue0ETv6Lmz0JKILkXatV33HOUVihFdAA19z8rdeHLguRnC9d22-1ud8w)**

<hr>
**Q8. **


**Q9. What is Classification ? What are the different tasks that take place in classification ?What are the different classification techniques **

*Ans*. **Classification** is a supervised learning technique in machine learning and data mining. It involves categorizing input data into classes or categories based on its characteristics or features. The goal is to develop a model that can accurately predict the class labels of new, unseen instances.

* Given a collection of records ( training set ) 
* Find a model for class attribute as a function of the values of other attributes
* Previously unseen records should be assigned a class as accurately as possible based on the training set.
**![](https://lh7-us.googleusercontent.com/SWf-iH76v7x_K9KbHJjF-Y5krXsPjBVDNmlT75YhmFh-jRA757oNjWgIoh_PsGkbePLCYBGHWYYClBPp03kvGneoGMi8MFJE2SJOFYaGAG0M1vsyGYc3kVq3aw25txdL6yN5SQarc_NKMx3yqUt6E7k)**

Classification Techniques
* Decision Tree based Methods
* Rule-based Methods
* Memory based reasoning
* Neural Networks
* Naive Bayes and Bayesian Belief Networks
* Support Vector Machines

<hr>

**Q10. Differentiate between Supervised and Unsupervised Learning**

*Ans*. Supervised vs. Unsupervised
Learning
**Supervised learning (classification)**
* Supervision: The training data (observations, measurements, etc.) are accompanied by labels indicating the class of the observations
* New data is classified based on the training set

**Unsupervised learning (clustering)**
* The class labels of training data is unknown
* Given a set of measurements, observations, etc. withnthe aim of establishing the existence of classes or clusters in the data

<hr>

**Q11. What are the different issues faced regarding classification and prediction ? **

*Ans*. 
1. *Data Preparation* : 
* Data cleaning
	* Preprocess data in order to reduce noise and handle missing values
* Relevance analysis (feature selection)
	* Remove the irrelevant or redundant attributes
* Data transformation
	* Generalize and/or normalize data
		* Numerical attribute income categorical {low,medium,high} 
		* Normalize all numerical attributes to [O, 1)

2. *Evaluating Classification Methods* :
* Predictive accuracy
* Speed
	* Time to construct the model
	* time to use the model
* Robustness
	* Handling noise and missing values
* Scalability
	* Efficiency in disk-resident databases
* Interpretability:
	* Understanding and insight provided by the model
* Goodness of rules (quality)
	* Decision tree size
	* Compactness of classification rules
