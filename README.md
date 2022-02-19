# Science Fair 2021-2022 - Predicting Human Behavior Buy/Sell Activities in Markets Using Deep Learning
# <img src="https://www.pngall.com/wp-content/uploads/4/Exclamation-Mark-Symbol-PNG.png" width="15" height="30" /> `WARNING: THIS IS NOT FINANTIAL ADVICE` <img src="https://www.pngall.com/wp-content/uploads/4/Exclamation-Mark-Symbol-PNG.png" width="15" height="30" />
This repository includes much of the code and information from the 2021-2022 Jasper High School Science Fair competition of Khosraw Azizi's project. Future developments to this project will be here.

<a href='https://ko-fi.com/khosraw' target='_blank'><img height='35' style='border:0px;height:46px;' src='https://az743702.vo.msecnd.net/cdn/kofi3.png?v=0' border='0' alt='Buy Me a Coffee at ko-fi.com/khosraw' />

	
### NOTE: The following datasets are under the Attribution-ShareAlike 4.0 International licence. For more information, visit: https://creativecommons.org/licenses/by-sa/4.0/legalcode

**Dataset Used:** https://drive.google.com/file/d/1AKyAxA1Alb1Lcq-VsAYEkkmljZm0yrun/view?usp=sharing

**Original Dataset:** https://www.kaggle.com/mczielinski/bitcoin-historical-data

## Abstract

The current Deep Learning difficulty with Machine Learning is the ability to make human behavior predictions. While Machine Learning has been able to make analytical predictions and judgments, it has not been able to reliably forecast a human's behavior to a circumstance. This minimizes the possibility for artificial intelligence to be used in a variety of fields. The problem may be solved by obtaining a large dataset of Bitcoin prices and passing it into a Google Collaboratory notebook using the Tensorflow framework and Pandas. The IBM Watson Tone Analyzer service may be used in conjunction with the Google News Python API to collect Bitcoin headlines throughout timeframes and utilize their data for model training and testing. The best model trained had a training MAE (mean absolute error) of 6.5, which translates to a 22 percent reduction in MAE, and the model had a testing MAE improvement of 61 percent with a testing loss of 11.9. When compared to an LSTM RNN (Recurrent Neural Network) model with a smaller dataset, the model improved testing loss by 225,164%. Applying RNN architecture to reduce loss, lowering the intervals between the important human behavior data obtained in the model, and using new and sophisticated architectures built for more effective training can all help to enhance the model if dealing with similar human behavior problems such as predicting other market values and monitoring the possible cardiac activity of a patient with cardiovascular diseases.

## Material

- Access to a Google Colab Notebook 
- Tensorflow 2.0 or newer 
- Matplotlib 
- Pandas 
- SkLearn
- IBM Watson Cloud account with the Tone Analyzer application (API Key & Application URL) 
- GoogleNews API
- The Kaggle Bitcoin dataset

## Procedure

1. Open a Google Colab notebook.
2. Retrieve the initial dataset for Bitcoin from the project GitHub repository or Kagle.
3. Upload the initial dataset for Bitcoin.
4. Install the ibm-watson library and pygooglenews API using pip.
5. Import all required libraries such as pygooglenews, datetime, json, numpy, pandas, and ibm_watson ibm_cloud_sdk_core.authenticators.
6. Create an instance of GoogleNews() as "gn".
7. Create a function to gather weekly news data by a given starting timestamp and use the GoogleNews API to gather search information as a string. Create arrays to store that information and use string modifiers alongside a for loop to modify all the data from the search. Assign numerical data using if statements based on the month the data is from. Convert the time given into UNIX timestamps using the timetuple() method. Follow that by returning all the gathered timestamps
8. Log into the previously created IBM Cloud account and open the Tone Analyzer to retrieve the API key and API URL.
9. Assign the API key and API URL to a variable and use IBM's authenticator to authenticate the use of the service. Also, assign the service as an object based on a specific version date of the service and an authenticator passed.
10. Create a function that loops through the previously created news data with timestamps and converts them to specific numerical values depending on the tone IBM Watson identifies it as. Break out the loop once the data is finished and return the entire data frame containing timestamps with their corresponding tone.
11. Import the dataset of the Bitcoin price data using Pandas and create an extra data sequence to put the tone data into.
12. Create a beginning timestamp to create the data.
13. Add the tone data into a data frame and give a position as a timestamp, loop through all the elements, and add the tone data to its corresponding array. Skip a specific amount of time in UNIX timestamps and after everything is put into arrays, break out of the loop.
14. Loop through the list of tones and add their values to the corresponding timestamp specified in the list of indexes.
15. Use the bfill() method to fill all the empty values in the column and then save the entire dataset as a CSV file using Pandas' data_to_csv() method. 
16. Proceed to create global variables for the horizon and the window size for the features.
17. Import matplotlib, sklearn.compose, and sklearn.preprocessing.
18. Create an optional callback function for Tensorboard by setting a location for the logs and saving the best checkpoints to be displayed in Tensorboard.
19. Create a checkpoint callback by setting a path for the checkpoints and saving the best epochs given the parameters to the ModelCheckpoint method.
20. Create a function to label the X and y values by dividing a specific number of X values into a specific number of y values based on the previously decided horizon and window size.
21. Create a function that gets all the values of the horizon based on a given window size by returning a list of X values to reach the y value.
22. Create a function to split the data into a train and test subset and determine that through a parameter that takes a percent of the data and changes it to test data.
23. Create a plotting function to take all the timestamps and their corresponding y values to plot the time and price of the dataset.
24. Begin to read the previously outputted dataset from the CSV file into a variable using Pandas.
25. Create a column transformer with a scaler for all the timestamps to normalize the values.
26. Set all the feature columns into a variable and set the label column into another variable.
27. Use the previously created column transformer to fit the features and labels.
28. Use the transform() method in the column transformer to normalize the features.
29. set all the timestamps into a variable and the label prie into another variable to be used for graphing.
30. Create a split size by taking the length of the list of prices and multiplying them by a given ratio.
31. Set X and y train variables using the split size.
32. Set X and y test variables using the split size.
33. Create an early stopping callback to monitor loss with the patience of 3.
34. Create the model using tf.keras.Sequential with 6 dense layers of reLU of 128 nodes, and an activation function of linear as output.
35. Compile the model with MAE being used for loss and the Adam optimizer being used with a learning rate of 0.00002.
36. Fit the model given the train data, batch size of 32, 15 epochs, and all callback functions.
37. Set the fit model into a variable. 
38. Evaluate the model by giving the evaluate() method test data and a batch size of 32.
39. Use the predict() method to predict all the label values given the features and enter them into a variable.
40. Save the model as a .h5 file format with the save() method.
41. Plot the entire data with its predictions by using the previously created plot function.
42. Plot the learning curve by turning the model's fit data put into a variable and using the plot() method to display it.
43. Display further plots of the predictions by setting different offsets to zoom into or out of the data.
	
## Graphs

### Graph of Dataset: 

![fab250fd-debc-43d0-8546-f3d2ca664513](https://user-images.githubusercontent.com/53713571/144168716-9edbbf5b-9ee8-40eb-9076-d8b20fe55605.png)

### Graphs of final product:
	
**Window 30, Horizon 1 (Using 30 minutes to predict 1 minute into the future)**
	
**Full Test Data Prediction Graph** ![download](https://user-images.githubusercontent.com/53713571/149870342-9f30775e-2c2b-49eb-81de-816cf76c6dd2.png)
	
**Testing Loss Graph** ![download](https://user-images.githubusercontent.com/53713571/149870381-0acd09cd-51d5-4e5a-bc47-09e96434cff7.png)
	
**Zoomed Test Data Prediction Graph** ![download](https://user-images.githubusercontent.com/53713571/149870395-ba25c39b-dcda-4f53-ae60-cb64cd866ca2.png)
	
**Further-Zoomed Test Data Prediction Graph** ![download](https://user-images.githubusercontent.com/53713571/149870401-d479d066-7a9d-4760-941f-70173db0d077.png)


## Error Analysis

Many important errors occur in the process of building a model. Firstly, a common error in time-series problems is not setting a window and a horizon. When windows and horizons are not set, the entire test data is used to predict one output value. This can cause inaccurate results since the entire dataset is influencing only one output. Utilizing a simple function to use indexing and break down the dataset into windows and horizons can make the results far more accurate.  

Additionally, batch size, which is responsible for the sample size of data the model trains from, can significantly affect the accuracy. While larger batch sizes lead to quicker mode training, they can also decrease the accuracy for some undiscovered reason. This high batch size was evident in the model created. High batch sizes for general testing purposes are fine, however, when collecting finalized data, it is important to decrease the batch size and be patient for the training to take place. There was a higher loss leading to less accurate results because the model specified a high batch size. This was solved by simply reducing the batch size to 32.

Finally, when dealing with any data that is not expected to be linear, an activation function must be set. Otherwise, the entire prediction of the graph will be using linear regression rather than unfixed points scattered throughout. Due to a lack of research and understanding of the data, this can often be a problem, which is why it's important to be able to visualize the data being passed and correlate it to a specific activation function. By understanding how to solve these issues and why they can occur, a lot of time can be saved while trying to build an efficient time-series model.

## Future Research & Application

By utilizing the method seen in this project to make more accurate predictions in time-series problems, many problems with the prediction of values involving human behavior factors can be solved. Companies, for example, can begin to use such significant human behavior variables in their services to allow investors to make more knowledgeable decisions on how to utilize their capital. However, further improvements can be made in other fields such as those in the medical field. This procedure can apply to the use of an ECG in a patient with cardiovascular conditions. More strokes can be averted ahead of time if a model can forecast certain heart rates based on historical data, such as physical and emotional activity. These forecasts can often be used to notify an individual of an imminent threat and to seek medical attention. This reduces the risk of a fatality, thus saving many lives from one of the greatest causes of death.

Further improvements to the model can be made by using RNN architecture to decrease loss even further. Decreasing the intervals between the relevant human behavior data gathered in the model can also allow more diverse data to decrease the loss of the model. More data can also be gathered as time passes to prepare the model in different instances. Furthermore, as new and complex architectures are created for more efficient training, multivariate models with the ability to predict human behaviors can lead to major solutions to real-world problems involving AI and Deep Learning.

## Conclusion

Khosraw Azizi

12.1.2021

**Predicting Human Behavior Buy/Sell Activities in Markets Using Deep Learning**
	
A major problem in current Deep Learning applications is their ability to make predictions involving human behavior. While Machine Learning has been able to make predictions and decisions analytically, it has not been able to predict a human's reaction to a given situation very accurately. For example, businesses go through many sudden changes, and because of the age of information, sources can report on those changes. These changes are then utilized by an audience that then reacts to that information, and makes changes to their investments, causing prices to fluctuate. The solution to this problem involves a multi-variate model that can train off of existing data based on human behavior, and then use pseudo-future test data to predict the future of a time-series problem. By utilizing this method, improvements can be made by decreasing testing loss by a significant amount in similar time-series problems. 

Firstly, to create a representation of a solution for such a problem, the project must be able to use existing data from a Bitcoin price dataset and add more data based on human behavior gathered from the numerical representation of a news article's tone regarding Bitcoin. The model may start by using an additional input dimension to create more accurate predictions about future Bitcoin values based on how the tone of a news piece impacts how humans invest in the past. The approach will entail obtaining a big dataset of Bitcoin prices and then loading the dataset onto a Google Collaboratory Notebook using the Tensorflow Python library and Pandas. The IBM Watson Tone Analyzer tool may be used in conjunction with the Google News Python API to collect Bitcoin headlines across periods and assess their tone in numerically represented data once there is a suitable dataset. This data will then be utilized to train an efficient dense Neural Network model, and the training and prediction outcomes of a model that does not include human behavior data will be compared. If there is a 10% decrease in loss, the human behavior data has a substantial influence on the forecasts. Using a GPU, the model must be able to train and assess in less than an hour. The MatPlotLib package may be used to graph all of the predictions alongside the graph of the real results from the pseudo-future test data prepared for evaluation once the predictions and evaluations for the model with human behavior data have been completed. All of this information may then be placed in a Pandas data frame and exported to a CSV file for further analysis. By using this method, significant improvements were observed compared to previous models. 
	
As a result of using the graphs, tables, and charts generated by the Colab notebook to evaluate the improvements from other pre-existing models, using multi-variate data for an extra layer of input made considerable improvements. Firstly, the best model trained resulted in a training MAE (mean absolute error) of 6.5, which evaluates to a 22% decrease in MAE compared to models not utilizing the generated tone data for multi-variation. In addition to the training improvements, the model had a testing MAE improvement of 61% with a testing loss of 11.9 when compared with the same model. The model also made a 225,164% improvement in testing loss when compared to a model utilizing an LSTM RNN (Recurrent Neural Network) model with the Yahoo Finance dataset and no tone data for multi-variation. These results lead to the conclusion that using data that can represent human behavior alongside a model for multi-variation can improve accuracy in predictions by a lot, especially because on average the training of the models took on average 53 minutes to occur while utilizing a CPU in the Google Collaboratory. 
	
By utilizing this method to make more accurate predictions in time-series problems, many problems with the prediction of values involving human behavior factors can be solved. Companies, for example, can begin to use such significant human behavior variables in their services to allow investors to make more knowledgeable decisions on how to utilize their capital. However, further improvements can be made in other fields such as those in the medical field. This procedure can apply to the use of an ECG in a patient with cardiovascular conditions. More strokes can be averted ahead of time if a model can forecast certain heart rates based on historical data, such as physical and emotional activity. These forecasts can often be used to notify an individual of an imminent threat and to seek medical attention. This reduces the risk of a fatality, thus saving many lives from one of the greatest causes of death. 
	
Further improvements to the model can be made by using RNN architecture to decrease loss even further. Decreasing the intervals between the relevant human behavior data gathered in the model can also allow more diverse data to decrease the loss of the model. More data can also be gathered as time passes to prepare the model in different instances. Furthermore, as new and complex architectures are created for more efficient training, multivariate models with the ability to predict human behaviors can lead to major solutions to real-world problems involving AI and Deep Learning.


## Annotated Bibliography

**A. Carter, D. S. A. S. (2016, March 10). Tensorflow — Neural Network Playground. Tensorflow Playground | GitHub. Retrieved September 22, 2021, from https://playground.tensorflow.org/** - The main purpose of the Tensorflow Playground is to be able to demonstrate different model hyperparameters easily to create an accurate evaluation. The website covers different hyperparameters, including batch size, dataset noise, activation function, learning rate, regularization, regularization rate, and problem type. This source allowed me to better understand what activation function to use when creating a regression model specific to my problem. However, it did not provide hyperparameter options for different optimization functions for optimizing the way the model learns. The source fits my attempt to choose an appropriate activation function by allowing me to model different activation functions that best fit my model problem.
	
**B. Goodfellow, I., Bengio, Y., & Courville, A. (2016). Deep Learning (Adaptive Computation and Machine Learning series) (Illustrated ed.) [E-book]. The MIT Press.** - The Deep Learning book by Goodfellow presents fundamental information for basic Linear Algebra and Calculus required in the back-end of deep learning. The book also presents basic information on the different types of deep learning models, and how each is different and useful to specific problems. By allowing me to understand specifically the difference between supervised learning, semi-supervised learning, and unsupervised learning. It fit my research as I required a basic understanding of the theory behind deep learning. While the book provided great detail into the mathematics and theory of all different model types, I only needed a basic understanding of deep learning.
	
**C. Google. (2021, April 22). All symbols in TensorFlow 2 | TensorFlow Core v2.6.1. TensorFlow. Retrieved September 19, 2021, from https://www.tensorflow.org/api_docs/python/tf/all_symbols** - The Tensorflow API documentation page for all symbols in the Tensorflow library provides all the different labels for classes and methods included in the library. The source does not include any detail as to the usage of any methods, examples of coding solutions, or an explanation of what they do. While the documentation page allowed me to have a reference as to all the different available methods, it did not provide information as to what they do or how to use them. Therefore, the source was a very basic documentation of what is included in the Tensorflow library in Python. 
	
**D. Google. (n.d.). Load CSV data | TensorFlow Core. TensorFlow. Retrieved September 25, 2021, from https://www.tensorflow.org/tutorials/load_data/csv** - The Tensorflow tutorial on loading data from a CSV file explained how to use a pandas method to load data into specific columns given a file path or URL as a parameter. To load a CSV file, one must use the pd.read_csv method from the Pandas library and pass a path as a parameter to the CSV file to load. The parameters may also include a list including the String corresponding to each column from left to right. This was relevant to my problem because before I was able to model and evaluate the problem, I had to load the large dataset from a CSV file. Through this information, I was able to load my Bitcoin dataset and separate the data into many columns. The source provided all the needed information for me to load CSV files in the Colab notebook, with more information on how to use the dataset inside an actual trained dense model.
	
**E. Grootendorst, M. (2021, December 29). 9 Distance Measures in Data Science | Towards Data Science. Medium. Retrieved January 13, 2022, from https://towardsdatascience.com/9-distance-measures-in-data-science-918109d069fa** - The Towards Data Science blog explains the 9 different distance measures, how they work, their pros, and their cons. When dealing with generally single-dimensional data, it is better to use a Euclidean Distance measure. However, if the vector contains multiple dimensions of data, distance measures such as the Cosine Similarity or the Manhattan Distance must be used to make calculations of distance. All other information provided by the source is for data that does not concern the data featured in this project. However, they have still been included in research in case the format of the data changes, especially as the model uses multi-variate data, and different dimensionalities can always be accounted for in the features of the model.
	
**F. IBM. (n.d.). Tone Analyzer - IBM Cloud API Docs. IBM Cloud. Retrieved November 14, 2021, from https://cloud.ibm.com/apidocs/tone-analyzer** - The IBM Cloud API documentation provided information regarding how to authenticate and use the IBM Watson Tone Analyzer service. It explained the usage of different server locations for the service URL to improve latency in HTTP responses. It also provided information on different response methods to be used after authenticating the API with the IAM Authenticator given an API key. Given this information, I was able to connect and send HTTP requests to the IBM Tone Analyzer service to receive responses on the tone from a given news headline. This helped add multi-variation to the model by adding an extra column to the dataset for the model to improve from. However, the documentation provided additional information on using JSON to get data from JSON response objects, but the information is not relevant to my problem.
	
**G. Jaquart, P. J., Dann, D. D., & Weinhardt, C. W. (2021, November 1). Short-term bitcoin market prediction via machine learning. ScienceDirect. Retrieved January 10, 2022, from https://www.sciencedirect.com/science/article/pii/S2405918821000027** - The Short-term bitcoin market prediction via machine learning project Patrick, David, and Christof, demonstrated the use of different model architectures while also displaying different horizons for the results. The model resulted in a 50% accuracy as it only predicts whether the price of Bitcoin will go up or down. The model also uses LSTM nodes in the RNN which could be a site for improvement in the current model of the project. Further information regarding the features used in the project and other model architectures demonstrated are included, However, they did not apply to this project while being a good frame of reference.
	
**H. Kotartemiy, K. (2020, June 30). GitHub - kotartemiy/pygooglenews: If Google News had a Python library. GitHub. Retrieved November 14, 2021, from https://github.com/kotartemiy/pygooglenews** - The Google News Python library documentation in the GitHub page for its repository, demonstrated how to install and use different methods from the library to get headlines. The main information that concerned my problem was the usage of the built-in search method used to receive a large number of news headlines. With the additional parameters for periods in the search method, I was able to search for headlines regarding Bitcoin between specific periods. The documentation contained several more methods and ways to create more search-specific headline lists, but I did not need that information for getting Bitcoin news headlines for tone analysis.
	
**I. M. (2020, November 22). GitHub - mrdbourke/tensorflow-deep-learning: All course materials for the zero to mastery deep learning with TensorFlow course. GitHub. Retrieved September 22, 2021, from https://github.com/mrdbourke/tensorflow-deep-learning** - The Tensorflow Deep Learning repository is for those who have participated in the Tensorflow Certification source. The GitHub repository contains Colab notebooks with theory and practical information on how to use Tensorflow. It specifically contained information about time-series problems, which allowed me to better shape my data to fit a time-series problem. I also utilized many important optimization methods, but the repository also includes information regarding projects, convolution, transfer learning, callbacks, natural language processing, classification models, and fundamental tensor modification. All of the information was relevant to my research excluding the majority of the information from the included natural language processing (NLP) notebooks used to create a project.
	
**J. Mueller, J. P., & Massaron, L. (2019). Deep Learning For Dummies (1st ed.) [E-book]. For Dummies.** - The Deep Learning For Dummies book by Mueller & Massaron demonstrates the fundamentals of both theory and practical ideas of Deep Learning. The book contains mathematical concepts such as matrices, vectors, and scalers. It also contains information regarding how to create and modify matrices using NumPy and Tensorflow. This information was the foundation of my background research as it helped me understand all the background processes that occur during a model's training and evaluation. However, I did not use the book to learn in-depth syntax as it was too detailed for my research timeframe. By understanding the basics of the Tensorflow library and Deep Learning, I could easily code a model while also being able to explain what the code executes.
	
**K. Shen, K. (2018, June 20). Effect of batch size on training dynamics - Mini Distill. Medium. Retrieved January 9, 2022, from https://medium.com/mini-distill/effect-of-batch-size-on-training-dynamics-21c14f7a716e** - The Medium article explores the effects of batch size on a model which was prompted by a major improvement of the currently developed model. Kevin Shen explores the fundamental unknown regarding why lower batch sizes result in better accuracy and also demonstrates the hypothesis of longer training time resulting in better accuracy. By using Kevin's data as a frame of reference, there was a better understanding of the effects of the batch size that was developed, and all the data was formatted to include information such as different learning rates, activation functions, training epochs, etc. While the article explores the effects of other super parameters such as learning rates and optimizers, the fundamental effects of batch size were the thing in question.
	
**L. Zielak. (2021, April 11). Bitcoin Historical Data. Kaggle. Retrieved October 7, 2021, from https://www.kaggle.com/mczielinski/bitcoin-historical-data** - The Bitcoin Historical Data dataset available at Kaggle by Zielak contained a large dataset of Bitcoin prices with 1-minute intervals in Unix timestamps. The dataset timeframe was from Jan 2012 to March 2021 and contained columns with the volume, open price, close price, high price, low price, etc. I was able to utilize this dataset for the entire project because it had a large amount of data. However, I cut down the data's timeframe to start from December of 2015, and I also removed all columns except the open price and the Unix timestamps corresponding with the price. This dataset was therefore used throughout the entire project and served as a placeholder for the final dataset used to contain an extra column for tone data for multi-variation modeling.
