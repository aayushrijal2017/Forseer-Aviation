# Forseer-Aviation
PS: Unzip the pickle file(file_rf) before running the model.
**Prerequisite:**
  1. Python Programming Language
  2. Knowledge of modules and libraries like Pandas, Seaborn, Matplotlib etc
  3. Machine learning Algorithm
  
<img width="943" alt="forseer aviation front page" src="https://user-images.githubusercontent.com/83895436/148351953-1264090d-6aa3-4da0-bdb6-51ec37219e0c.PNG">


**Academic Project : An Artificial Intelligent Platform to Predict the flight Fares.**

 In this project I have implemented Machinelearning algorithm to predict the flight fare. The steps involved in the projects are:
 
   1. **Data Collection/ gathering.**
   
    One of the quickest and easiest way to get the sample data is a platform name "Kaggle". I have downloaded the data set from Kaggle. The respective link is given below:
      https://www.kaggle.com/nikhilmittal/flight-fare-prediction-mh
      
      <img width="708" alt="kaggle" src="https://user-images.githubusercontent.com/83895436/148352704-3ada44a0-df2e-4d58-957f-8b968c767147.PNG">
      
    The train and test data sets are separated in different files so that we can preprocess and apply our algorithm separately.
    
  2. **Data Cleaning.**
  
        As a machine learning Engineer, by obtaining those data my first and foremost step was to clean the data.
        I became familiar with domain knowledge by reading the vlogs and started to clean the data.
        First of all, relevant modules like seaborn, pandas, Matplotlib etc were imported.
        
        <img width="863" alt="modules and packages" src="https://user-images.githubusercontent.com/83895436/148353725-07d4ebcf-1ed3-4eb2-ac9f-20adbe3da983.PNG">
        
        Necessary things to keep in mind are:
        1. Since this is manmade dataset, there might be humans errors.
        2. Each and Every columns required for us should be preprocessed or unnecessary column can be discarded. This help to reduce the dimension of our dataset.
        3. Null values present in the columns were assigned to 0 or respective data types.
    
  3. **Exploratory Data Analysis**    
  
       Relevent Columns like Journey day, Journey month, Source, Destination, Airlines, Prices were the prime columns to determine the price prediction.
        
        Each Columns is processed and analysed individually.
        
        <img width="842" alt="data" src="https://user-images.githubusercontent.com/83895436/148356411-189e189c-0009-4d8a-9fdb-39528f7fd2e5.PNG">

      Data is visaulised using different plots, I used some of the plotting techniques to observe the data. Example is shown below:-
      
      <img width="837" alt="data visualization" src="https://user-images.githubusercontent.com/83895436/148356909-58b60955-81b4-43a4-ad89-e1d50b8d1fe4.PNG">
<img width="832" alt="catplot" src="https://user-images.githubusercontent.com/83895436/148357252-8c238d50-a563-4aaa-8b62-24a109a68f03.PNG">

     Categorical Data should be handled properly.
     
      The different types of data are:

         a.Nominal data ---> data that are not in any order --->OneHotEncoder is used in this case
         
         b.Ordinal data ---> data that are in order ---> LABELENCODER is used in this case
 
   ****Similarly same steps were used for Test data Set as well****

 4. **Feature Selection**

    Feature selection is the process of reducing the number of input variables when developing a predictive model.
    It is desirable to reduce the number of input variables to both reduce the computational cost of modeling and, in some cases, to improve the performance of the model.
    
    There are two main types of feature selection techniques: supervised and unsupervised, and supervised methods may be divided into wrapper, filter and intrinsic.
    
    Filter-based feature selection methods use statistical measures to score the correlation or dependence between input variables that can be filtered to choose the most relevant features.
    Statistical measures for feature selection must be carefully chosen based on the data type of the input variable and the output or response variable.
 
    For this Project I have used Heatmap which helped me to identify the correlation between independent and dependent features.
    
    a. Extratree Regressor is used. This class implements a meta estimator that fits a number of randomized decision trees (a.k.a. extra-trees) on various sub-samples of the        dataset and uses averaging to improve the predictive accuracy and control over-fitting.
    
    b.  Hyper parameter Tuning is done by randomized Search CV.
    
        Hyperparameters are crucial as they control the overall behaviour of a machine learning model. 
     
        The ultimate goal is to find an optimal combination of hyperparameters that minimizes a predefined loss function to give better results.
        
   5. **ML model**
  
       I have used pickle to keep the model in a file so that next time I don't have to go through each and every steps. By the help of the pickle file I can run my model without doing above steps.Thus, it increases resuability of my code.
       
       <img width="551" alt="pickle" src="https://user-images.githubusercontent.com/83895436/148359418-292d3139-9a42-4f95-9191-0e514a196e63.PNG">

6. **Production of ML model**
      
      By the help of the HTML and CSS skills. I have designed a simple website which I have shown below:
      
      <img width="943" alt="forseer aviation front page" src="https://user-images.githubusercontent.com/83895436/148359687-7ad80b68-f73c-42be-b5bf-2366862df6d3.PNG">
      
      <img width="941" alt="lower aviation" src="https://user-images.githubusercontent.com/83895436/148359711-5c5fa751-75f0-4031-9604-2ed1e6dfb596.PNG">
      
      User can input their desired date of journey, they will be able to choose the airlines, Stoppage and can predict the fare of the Airlines.
      
      In the example I have used the following queries:
      SOURCE : Dehli
      Destination: Cochin
      Stoppage : Non-Stop
      Airlines: Indigo 
      Departure Date : Relevant
      And predict button is clicked.
      
     The price is predicted for the respective query was INR 5669. 

<img width="900" alt="prediction" src="https://user-images.githubusercontent.com/83895436/148361327-f3ba5505-7696-4092-bdf5-7c247b389592.PNG">

 



