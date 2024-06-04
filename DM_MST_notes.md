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

## Exam Questions

**Q1. What is Data Mining and why do we do it ? Give some  uses of data mining and examples of data mining applications**

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

**Q. What is data ? Define types of attributes and their properties ?**

*Ans*. Data is basically a collection of data objects and their attributes.
* An attribute is a property or characteristic of an object.
	* It is also known as *variable, field, characteristic or feature*
	* Ex : eye color of a person, temperature, etc
* A collection of attributes describe an object.
	* An obejct is also known as a record, sample or entity.

There are mainly 4 types of attributes : __NOIR__
* Nominal ( 1 ) : 
	* Simplest level and are categories with no ranking or order.
	* Ex : Id numbers, zip codes, etc
* Ordinal ( 1 & 2) : 
	* They can be arranged in meaningful order
	* Ex : rankings ( scale of 1 to 10 )
* Interval : ( 1, 2 & 3 ) : 
	* Ordered categories and meaningful differences between values
	* Ex : calendar dates, temp in *C or farenheit
* Ratio : ( 1, 2, 3 & 4 ) : 
	* Highest level of measurement, with both differences and ratios being meaningful
	* Ex : Length, time, counts, etc

These attributes can possess the following properties > 
1. Distinctiveness
2. Order
3. Addition 
4. Multiplication

Attributes can be of 2 types : 
Discrete Attribute
* Has a finite or countably infinite set of values
* Often represented as integer variables'

Continuous Attribute
* Has real numbers as attribute values
* Can only be measured and represented using a finite set of digits.
* Represented as floating point variables

<hr>

**Q. What are the different types of Datasets ?**

*Ans*. There are mainly 3 types of datasets : __ROG__
* *Record*
Data organized in rows or records, where each record represents an individual entity
	* Data matrix
	* Document data
	* Transaction data
* *Ordered*
Data arranged in a specific sequence or order, often with a defined relationship between consecutive elements
	* Spatial Data
	* Temporal Data
	* Sequential Data
	* Genetic Sequence Data
* *Graph*
Data structured as a graph consisting of nodes (entities) and edges ( relationships between them )
	* WWW
	* Molecular Structures

<hr>

**Q. What is Data Quality?**

*Ans*. Data quality is  a measure of how suitable data is for the purpose of data mining.	
To get data of good quality from databases we need to look at the following questions : 
* What kinds of data quality problems are there?
* How do we detect problems with the data ?
* What can we go about these problems ?

Some of the data quality problems are as follows : 
1. Noise
**![](https://lh7-us.googleusercontent.com/kMLO2ZBODA6eilewvzUEDODwY_auoBIV8_mJBaHVFM_yF4z70SlaJtCUtAwZkfnvnehIy9AOqG6dcgd4m4n8uh0Jq560nYaIOH_puks0LhM0EWgO9EoHMxxydISPEzO0rsZFt-IsGXUujAZ1oAolknM)**
* This refers to the modification of the original values.

2. Outliers 
**![](https://lh7-us.googleusercontent.com/ix2j-r7koJSig0lu59AFdnfkNqucelFAICIUCsADT46GBKTatlAd_ukki4o1PpThnJ4AKMCWD3dDlgyx_3lM0AsFSuTycznaFNMKVWSE9168IAN-1u-2gNdR9ZNG6xXJf4YHl-PcJsvFu1pJUPU90e4)**
* There are data objects with characteristics that are *considerably* different from most of the other data objects in the data set

3. Missing Values : 
* Reasons for missing values : 
	* Information isn't collected
	* Attributes may not be applicable to all cases
* Handling Missing Values : 
	* Eliminate Data Objects
	* Eliminate missing values
	* Ignore the missing values during analysis
	* Fill the missing attributes with the most probable values.

4. Duplicate Data
* Data set may include objects that are duplicates or extremely close to being identical
	* Major issues arise when merging data from heterogeneous sources.

<hr>

**Q.What is Data Preprocessing ?**

*Ans* Data preprocessing is a critical step in data analysis and machine learning workflows. It involves cleaning, transforming, and organizing raw data into a format suitable for analysis or modeling.
__ASDFFDA__

* Aggregation : 
	* Combining two or more attributes into a single attribute.
	* Done for data reduction and to get more stable data
* Sampling : 
	* Selecting a subset of datapoints from the larger dataset 
	* Done because using the entire dataset would be too expensive and time consume
		* Simple random sampling
		* Sampling without replacement
		* Sampling with replacement
		* Stratified sampling
* Dimensionality Reduction : 
	* Reducing the number of variables in the dataset
	* This can be done with the help of PCA, Singular value decomposition ( SVD ), etc
* Feature subset selection
* Feature creation
* Discretization and binarization : 
	* Converting continuous variables into discrete variables.
* Attribute transformation : 
	* Transforming the scale, distribution or nature of the attributes.
	* This can be done with the help of normalization, standardization, logarithmic transformation, etc

<hr>

**Q. What is association rule mining ? What is a frequent itemset ? Define the different association rule mining tasks**

*Ans*. 
Given a set of transactions, finding the rules that will predict the occurence of an item based on the occurences of other items is called association rule mining.
**![](https://lh7-us.googleusercontent.com/8h9A3gq2Hk2g4mAuZu2kruf-CMw1bi4vGh5AxMhFAo17ptIIS_jf4XX5mV6NI3x7zLn7lG22LyWEofzEFKaET9V7qeAimrS4zzW2i_jg2Lv-pRYMCGdvyWGpVn-CwN5aYJZXi3uMp4PVoxPOX5Qws5s)**
Example of Association Rules
{Diaper} —> {Beer},
{Milk, Bread} —>{Eggs,Coke},
{Beer, Bread} —>{Milk}

**Frequent Itemset** : __ISSFAR__
* Itemset : 
	* It is a collection of one or more items
* Support Count :
	* Frequency of occurence in an itemset
* Support :
	* Fraction of transactions that contain an itemset
* Frequent Itemset :
	* An itemset whose support is greater than or equal to a minsup threshold
* Association Rule : 
	* An expression of the form X --> Y where X and Y are itemsets.
* Rule evaluation metrics : 


<hr>

**Q. What are the steps taken in the process of KDD?**

*Ans*.
#### Knowledge Discovery of Databases
KDD is a process that involves discovery / extraction of useful information ( previously unknown and potentially valuable ) from large datasets.
* It is a multiple step process, and Data Mining is one of those steps 
* The Process of knowledge discovery in data mining follows the given set of steps :

1.Data Selection : 
* It is defined as the selection of relevant subset of the dataset for analysis.

2.Data Cleaning : 
* It is the removal of noise or irrelevant data in the selected dataset.
* Various methods are used to get rid of noise, outliers, missing data and duplicate data.

3.Data Integration : 
* This heterogenous data is the stored into a data warehouse.
* Integration is done by data integration tool

4.Data Transformation and Reduction : 
* In this step the data is transformed into a  homogeneous format.
Helps in dimensionality reduction as well

5.Data Mining : 
* It is the core process of KDD
* You can you either of the following functions of KDD
	* Summarization
	* Classification
	* Regression
	* Association
	* Clustering

6.Pattern Evaluation : 
* Extracting useful and strong patterns in the data
* Making decisions

7.Knowledge Representation : 
* Using visualization tools to disply the extracted patterns.
* 
**![](https://lh7-us.googleusercontent.com/1PeOBbWmnK-eLkeRZj2eBh3Sn2UHFd3af9Orgrv26plnQ8XZlu72C2qtP3R282c_ftzcPyFLkxZ3k_JuENOiZRmWI04AhFqIpth2BPknE-0BgJCRL_1zoRMzStBJ-3a7zv6h2btzzcERgtP2Csispio)**

<hr>

**Q.   What are the different data mining tasks? Note the difference data mining methods**

*Ans*. The difference data mining tasks are as follow : 
* __Classification__  : Leaning a function that maps an item into a set of predefined classes.
* __Regression__ : Learning a function that maps an item to a real value.
* __Clustering__ : Identify a set of groups of similar items .
* __Dependency and Associations__ : Identify any *significant dependencies* between data *attributes*.
* __Summarization__ : To find a compact decription of the dataset.

<hr>

**Q. Why not traditional data analysis ?**

*Ans* The use of traditional data analysis techniques has been reduced for the following reasonss : 
* Tremendous amounts of data 
	* Algorithms must be scalable so as to handle tera-butes of data
* High dimensionality 
	* A singular micro array may have tens of thousands of dimensions
* HIgh complexity of data
* New and sophisticated applications

<hr>

**Q. On what kinds of applications can you do data mining ?**

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

**Q. What are the different Data Mining Functionalities ?**

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

**Q. What are the Major issues in Data Mining ?**

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

**![](https://lh7-us.googleusercontent.com/MqoMkeXOG0qegkDjw5qhbF6fM4WozwKSM-ZIytvArZdinzaGYV_jQNCkTmEb91TPzQoTrU_tghE0DW8p5zqPgDPkO1-iT_6pybB0jtOrVnuC_BboqE4hpXOLJs8SbavTrFxQm0T1ycQJ6y1HsdelHvw)**

<hr>


**Q. What is Classification ? What are the different tasks that take place in classification ? What are the different classification techniques**

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

**Q. Differentiate between Supervised and Unsupervised Learning**

*Ans*. Supervised vs. Unsupervised
Learning
**Supervised learning (classification)**
* Supervision: The training data (observations, measurements, etc.) are accompanied by labels indicating the class of the observations
* New data is classified based on the training set

**Unsupervised learning (clustering)**
* The class labels of training data is unknown
* Given a set of measurements, observations, etc. withnthe aim of establishing the existence of classes or clusters in the data

<hr>

**Q. What are the different issues faced regarding classification and prediction ?**

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

<hr>

**Q12. What are decision trees ?**

*Ans*. Decision trees are used to represent learned target functions
- Each internal node tests an attribute
- Each branch corresponds to attribute value
- Each leaf node assigns a classification
- Can be represented by logical formulas

**![](https://lh7-us.googleusercontent.com/doJPcVzHEIRWnLsXJ08x1K2X7GWPFGBlB0IC8sVbbuqtvgNC-v7sa3gOrfX-BqdkCcfCxMcrapqSEuQqGY7Pv69bTGoTNW9AASpAdILRJdHF_ufrlBqDWtAnDqXmxrp0xDLjjFu9-rhBNc46kDrsU4o)**
