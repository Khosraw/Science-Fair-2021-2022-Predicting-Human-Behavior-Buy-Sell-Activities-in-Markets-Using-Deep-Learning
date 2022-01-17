# Science Fair 2021 - Predicting Human Behavior Buy/Sell Activities in Markets Using Deep Learning
# <img src="https://www.pngall.com/wp-content/uploads/4/Exclamation-Mark-Symbol-PNG.png" width="15" height="30" /> `WARNING: THIS IS NOT FINANTIAL ADVICE!`
This repository includes much of the code and information from the 2021-2022 Jasper High School Science Fair competition of Khosraw Azizi's project. Future developments to this project will be here.

<a href='https://ko-fi.com/khosraw' target='_blank'><img height='35' style='border:0px;height:46px;' src='https://az743702.vo.msecnd.net/cdn/kofi3.png?v=0' border='0' alt='Buy Me a Coffee at ko-fi.com/khosraw' />

	
### NOTE: The following datasets are under the Attribution-ShareAlike 4.0 International licence. For more information, visit: https://creativecommons.org/licenses/by-sa/4.0/legalcode

**Dataset Used:** https://drive.google.com/file/d/1cslRLdDsJlf-krQg-lzcqrClaYgE2gJi/view?usp=sharing

**Original Dataset:** https://www.kaggle.com/mczielinski/bitcoin-historical-data

## Abstract

The current Deep Learning problem with Machine Learning is the application's ability to make human behavior predictions. While Machine Learning has been able to make analytical predictions and judgments, it has not been able to reliably forecast a human's behavior to a circumstance. This minimizes the possibility for artificial intelligence to be used in a variety of fields. The problem may be solved by obtaining a large dataset of Bitcoin prices and loading it into a Google Collaboratory using the Tensorflow framework and Pandas. The IBM Watson Tone Analyzer service may be used in conjunction with the Google News Python API to collect Bitcoin headlines throughout timeframes and utilize their data for model training and testing. The best model trained had a training MAE (mean absolute error) of 6.3, which translates to a 27 percent reduction in MAE, and the model had a testing MAE improvement of 22 percent with a testing loss of 24. Applying RNN architecture to reduce loss, even more, lowering the intervals between the important human behavior data obtained in the model, and using new and sophisticated architectures built for more effective training can all help to enhance the model if dealing with similar human behavior problems.

## Material

- A PC:
  - Processor - AMD Ryzen 5 4500U with Radeon Graphics (6) @ 2.375GHz (6 Cores | 12 Threads)
  - Installed RAM - 8.00GB
  - 1 TiB SSD
  - System Type: 64-Bit, x64-based processor
  - OS: Linux Kernel 5.15.8-Zen of GNU/Linux (Can be Windows)
  - Distribution: Archcraft
  - Has Access to a Stable WIFI Connection
  - Contains a web browser (Vivaldi)
- Email Account (khosraw.azizi@gmail.com | Recommended no school, work, or organization email addresses)
- Website - colab.research.google.com, https://github.com/Khosraw/Science-Fair-2021---Predicting-Human-Behavior-Buy-Sell-Activities-in-Markets-Using-Deep-Learning

## Procedure

1. Plug in the laptop's charging cord into a power socket and the other end of the power cord into the laptop's charging port.
2. Press the power button on the computer.
3. If the material involves Windows or if there is no duel booting (running multiple operating systems at the same time), skip to step 4. Otherwise, use the arrow keys to navigate to the proper operating system and press the enter key on the keyboard.
4. If prompted to enter a password to log in, enter the password using the keyboard.
5. Once logged in, if on Windows, press the Windows/Super key and type the name of the browser that will be used. If on Linux with Archcraft, press the Windows/Super key and type the exact name of the browser, and then press enter to open it. If using any other Linux distribution, the process will always vary depending on the distribution.
6. If on Windows, check the bottom right corner of the screen to see if the WIFI symbol has full or partially full white bars. If yes, skip to step 7. If no, click on the WIFI symbol to open up the WIFI menu, and then click the WIFI connection chosen to connect to, and if required a passcode, enter the passcode using the keyboard and press the enter key. If on Archcraft Linux, check the top bar for the WIFI symbol and see if the WIFI symbol is crossed out and/or is red. If no, skip to step 7. If yes, press the Windows/Super key with the N key to open up the WIFI menu. Once open in the menu, use the up and down arrow keys to navigate up and down the connections list, or use left and right to go through the different pages. If asked for a passcode, use the keyboard to enter it and press enter.
7. Once the browser is open, click on the top empty search bar.
8. Once the cursor in the search bar starts blinking, type in the following link into it using the keyboard, and then press enter: https://github.com/Khosraw/Science-Fair-2021---Predicting-Human-Behavior-Using-Deep-Learning-Market-Prediction
9. Once the page is fully loaded, see the box labeled at the top as "README.md", scroll down until the text labeled "Dataset Used:" can be seen, and middle-click on the link to the right of that text.
10. If the new tab cannot be seen on screen, see the top bar of the browser where tabs are listed and click on the one labeled with "output.csv". Otherwise, click on the button labeled "Download", and save the file to a location on the computer. 
11. Switch back to the tab with the GitHub page labeled with "Khosraw".
12. Look through the top box where files are listed, and click on the file labeled "SF_TF_BTC_Final.ipynb" on the left side of the box.
13. If the page is loaded to a website linked colab.research.google.com shown at the top of the browser (the address/search bar) and there is no button on the top right of the page labeled Sign In, skip to step 17. Otherwise, click on the Sign In button on the top right.
14. If the page contains an available list of accounts, click on the preferred account and skip to step 15. If not, click on the empty box for the emails and type in the full email address for the account, and then click on the button labeled Next. 
15. Click on the empty box for the password field and enter the password for the corresponding email address chosen previously, and click the button labeled Next.
16. If asked to use Two-Factor authentication, proceed with the preferred way to authenticate the account. Otherwise, skip to step 17.
17. Identify the top row of buttons in the Colab website labeled with File, Edit, View, Insert, Runtime, Tools, and Help.
18. Hover the mouse over the Runtime item in the top row and click on it.
19. Hover the mouse over the "Change runtime type" and click on it.
20. Once a box labeled "Notebook settings" appears, click on the dropdown menu below the label titled "Hardware accelerator", and click on the item labeled GPU. 
21. Once set, click on the button labeled "Save".
22. Identify the Folder/File icon on the left side of the page and hover the mouse over it to then click on the button.
23. Once the "Files" tab expands, click on the button with the file icon and an arrow pointing upwards inside the icon to upload a file. 
24. Navigate to the location where the previously downloaded "output.csv" is, and double click it to upload it to Colab.
25. If a window labeled with "Reminder, uploaded files will get deleted when this runtime is recycled." opens, click on the button labeled "OK". Otherwise, skip to step 26.
26. Click on the top row button labeled Runtime and click on the button labeled "Run all".
27. If a window titled "Warning: This notebook was not authored by Google." comes up, click on the button labeled "Run anyway" to proceed. Otherwise, skip to step 28.
28. Use the scroll wheel on a mouse or two fingers to scroll down the page until the output is visible with outputs such as "Epoch 1/100".
29. Observe the loss/mae (mean absolute error) of each epoch being displayed until the model stops training.
30. When a graph is displayed at the end of the output box, it means that the model is done training. Observe the graphs, along with the final training loss/mae at the last labeled epoch, and observe the final row of evaluation where the output states with "62/62" for the testing loss/mae. 
31. Using the previously observed testing loss/mae value, record that the final predictions for the trained model are on average loss/mae dollars off the true pseudo-future values (Ex: $26.96 off since the loss/mae value is 26.9553).
32. Check the Files panel on the left of the site which was opened previously and identify the file labeled "Bitcoin Data Predictions.csv".
33. Right-click on the file and click on the button labeled "Download" on the menu.
34. Save the file locally and open it in either an official CSV-supported application or in a simple text editor like Geany (Linux) or Notepad (Windows).
35. Make observations based on the left column and the right column. How close are the predictions to the actual open prices of Bitcoin?
	
## Graphs

### Graph of Dataset: 

![fab250fd-debc-43d0-8546-f3d2ca664513](https://user-images.githubusercontent.com/53713571/144168716-9edbbf5b-9ee8-40eb-9076-d8b20fe55605.png)

### Graphs of final product:
	
**Window 7, Horizon 1 (Using 7 days to predict 1 day into the future)**
	
![image](https://user-images.githubusercontent.com/53713571/146692062-4cd54d97-3376-45f0-be66-100df4d1c1ee.png)
![image](https://user-images.githubusercontent.com/53713571/146692068-98950147-c87d-4c1f-b247-22df3cb58f4a.png)
![image](https://user-images.githubusercontent.com/53713571/146692070-92e62c78-c783-4f82-8af3-fd533f285701.png)
![image](https://user-images.githubusercontent.com/53713571/146692073-187e796d-1543-4e95-b949-779ea33a2cfd.png)
	
**Window 7, Horizon 2 (Using 7 days to predict 2 days into the future & 1 day into the future | orange line for 1 day, green line for 2 days)**
	
![image](https://user-images.githubusercontent.com/53713571/146692079-29716f2e-6d64-4312-9c8d-381054f45165.png)
![image](https://user-images.githubusercontent.com/53713571/146692080-e982faa8-0ea0-4073-8546-7a5f1a72d6ee.png)
![image](https://user-images.githubusercontent.com/53713571/146692085-ef942d0b-84de-4c58-a905-fcefc10fec80.png)
![image](https://user-images.githubusercontent.com/53713571/146692089-78b7a9fd-9bcf-400d-8efc-5ec3970d3ff7.png)

## Error Analysis

Many important errors occur in the process of building a model. Firstly, a common error in time-series problems is not setting a window and a horizon. When windows and horizons are not set, the entire test data is used to predict one output value. This can cause inaccurate results since the entire dataset is influencing only one output. Utilizing a simple function to use indexing and break down the dataset into windows and horizons can make the results far more accurate.  

Also, a rather dangerous mistake can be uploading the API key for the API that is being used publicly such as GitHub. This can quickly get the account from which the API key is owned from being abused, using up all the API requests available. It is best practice to double-check for API keys or use GitHub Guardian to automatically detect leaked security flaws or API keys.  

Finally, when dealing with any data that is not expected to be linear, an activation function must be set. Otherwise, the entire prediction of the graph will be using linear regression rather than unfixed points scattered throughout. By understanding how to solve these issues and why they can occur, a lot of time can be saved while typing to build an efficient Neural Network.

## Future Research & Application

By utilizing the method seen in this project to make more accurate predictions in time-series problems, many problems with the prediction of values involving human behavior factors can be solved. Many companies for example can begin to use such significant human behavior variables in their services to allow investors to make more knowledgeable decisions on how to utilize their capital. However, further improvements can be made in other fields such as those in the medical field. This procedure, for example, can be used to perform an ECG. More strokes can be averted ahead of time if a model can forecast certain heart rates based on historical data, such as physical and emotional activity. This reduces the risk of a fatality, thus saving many lives.

Further improvements to the model can be made by using RNN architecture to decrease loss even further. Decreasing the intervals between the relevant human behavior data gathered in the model can also allow more diverse data to decrease the loss of the model, and as new and complex architectures are created for more efficient training, multivariate models with the ability to predict human behaviors can lead to major solutions to real-world problems involving AI and Deep Learning.

## Conclusion

Khosraw Azizi

12.1.2021

**Predicting Human Behavior Using Deep Learning & News Headlines For Bitcoin Price Prediction - Conclusion**

A major problem in current Deep Learning applications is the ability to make predictions involving human behavior. While Machine Learning has been able to make predictions and decisions analytically, it has not been able to predict a human's reaction to a given situation very accurately. For example, businesses go through many sudden changes, and because of the age of information, sources can report on those changes. These changes are then utilized by an audience that then reacts to that information, and makes changes to their investments which causes prices to fluctuate. The solution to this problem involves a multi-variate model that can train off of existing data based on human behavior, and then use pseudo-future test data to predict the future of a time-series problem. By utilizing this method, improvements can be made by decreasing testing loss by a significant amount in similar time-series problems.
	
Firstly, to create a representation of a solution for such a problem, the project must be able to use existing data from a Bitcoin price dataset and add more data based on human behavior gathered from the numerical representation of a news article's tone regarding Bitcoin. The model may start by using an additional input dimension to create more accurate predictions about future Bitcoin values based on how the tone of a news piece impacts how humans invest in the past. The approach will entail obtaining a big dataset of Bitcoin prices and then loading the dataset onto a Google Collaboratory Notebook using the Tensorflow Python library and Pandas. The IBM Watson Tone Analyzer tool may be used in conjunction with the Google News Python API to collect Bitcoin headlines across periods and assess their tone in numerically represented data once there is a suitable dataset. This data will then be utilized to train an efficient dense Neural Network model, and the training and prediction outcomes of a model that does not include human behavior data will be compared. If there is a 10% increase in accuracy, the human behavior data has a substantial influence on the forecasts. Using a GPU, the model must be able to train and assess in less than an hour. The MatPlotLib package may be used to graph all of the predictions alongside the graph of the real results from the pseudo-future test data prepared for evaluation once the predictions and evaluations for the model with human behavior data have been completed. All of this information may then be placed in a Pandas data frame and exported to a CSV file for further analysis. By using this method, significant improvements were observed compared to previous models.
	
As a result of using the graphs, tables, and charts generated by the Colab notebook to evaluate the improvements from other pre-existing models, using multi-variate data for an extra layer of input made considerable improvements. Firstly, the best model trained resulted in a training MAE (mean absolute error) of 6.3, which evaluates to a 27% decrease in MAE compared to models not utilizing the generated tone data for multi-variation. In addition to the training improvements, the model had a testing MAE improvement of 22% with a testing loss of 24 when compared with the same model. The model also made a 111,644% improvement in testing loss when compared to a model utilizing an LSDM RNN (Recurrent Neural Network) model with the Yahoo Finance dataset and no tone data for multi-variation. These results lead to the conclusion that using data that can represent human behavior alongside a model for multi-variation can improve accuracy in predictions by a lot, especially because on average the training of the models took on average 18 minutes to occur while utilizing a GPU in the Google Collaboratory. 
	
By utilizing this method to make more accurate predictions in time-series problems, many problems with the prediction of values involving human behavior factors can be solved. Many companies for example can begin to use such significant human behavior variables in their services to allow investors to make more knowledgeable decisions on how to utilize their capital. However, further improvements can be made in other fields such as those in the medical field. This procedure, for example, can be used to perform an ECG. More strokes can be averted ahead of time if a model can forecast certain heart rates based on historical data, such as physical and emotional activity. This reduces the risk of a fatality, thus saving many lives.
	
Further improvements to the model can be made by using RNN architecture to decrease loss even further. Decreasing the intervals between the relevant human behavior data gathered in the model can also allow more diverse data to decrease the loss of the model, and as new and complex architectures are created for more efficient training, multi-variate models with the ability to predict human behaviors can lead to major solutions to real-world problems involving AI and Deep Learning.

## Annotated Bibliography

**A. Carter, D. S. A. S. (2016, March 10). Tensorflow — Neural Network Playground. Tensorflow Playground | GitHub. Retrieved September 22, 2021, from https://playground.tensorflow.org/** - The main purpose of the Tensorflow Playground is to be able to demonstrate different model hyperparameters easily to create an accurate evaluation. The website covers different hyperparameters, including batch size, dataset noise, activation function, learning rate, regularization, regularization rate, and problem type. This source allowed me to better understand what activation function to use when creating a regression model specific to my problem. However, it did not provide hyperparameter options for different optimization functions for optimizing the way the model learns. The source fits my attempt to choose an appropriate activation function by allowing me to model different activation functions that best fit my model problem.

**B. Goodfellow, I., Bengio, Y., & Courville, A. (2016). Deep Learning (Adaptive Computation and Machine Learning series) (Illustrated ed.) [E-book]. The MIT Press.** - The Deep Learning book by Goodfellow presents fundamental information for basic Linear Algebra and Calculus required in the back-end of deep learning. The book also presents basic information on the different types of deep learning models, and how each is different and useful to specific problems. By allowing me to understand specifically the difference between supervised learning, semi-supervised learning, and unsupervised learning. It fit my research as I required a basic understanding of the theory behind deep learning. While the book provided great detail into the mathematics and theory of all different model types, I only needed a basic understanding of deep learning.

**C. Google. (2021, April 22). All symbols in TensorFlow 2 | TensorFlow Core v2.6.1. TensorFlow. Retrieved September 19, 2021, from https://www.tensorflow.org/api_docs/python/tf/all_symbols** - The Tensorflow API documentation page for all symbols in the Tensorflow library provides all the different labels for classes and methods included in the library. The source does not include any detail as to the usage of any methods, examples of coding solutions, or an explanation of what they do. While the documentation page allowed me to have a reference as to all the different available methods, it did not provide information as to what they do or how to use them. Therefore, the source was a very basic documentation of what is included in the Tensorflow library in Python. 

**D. Google. (n.d.). Load CSV data | TensorFlow Core. TensorFlow. Retrieved September 25, 2021, from https://www.tensorflow.org/tutorials/load_data/csv** - The Tensorflow tutorial on loading data from a CSV file explained how to use a pandas method to load data into specific columns given a file path or URL as a parameter. To load a CSV file, one must use the pd.read_csv method from the Pandas library and pass a path as a parameter to the CSV file to load. The parameters may also include a list including the String corresponding to each column from left to right. This was relevant to my problem because before I was able to model and evaluate the problem, I had to load the large dataset from a CSV file. Through this information, I was able to load my Bitcoin dataset and separate the data into many columns. The source provided all the needed information for me to load CSV files in the Colab notebook, with more information on how to use the dataset inside an actual trained dense model.

**E. IBM. (n.d.). Tone Analyzer - IBM Cloud API Docs. IBM Cloud. Retrieved November 14, 2021, from https://cloud.ibm.com/apidocs/tone-analyzer** - The IBM Cloud API documentation provided information regarding how to authenticate and use the IBM Watson Tone Analyzer service. It explained the usage of different server locations for the service URL to improve latency in HTTP responses. It also provided information on different response methods to be used after authenticating the API with the IAM Authenticator given an API key. Given this information, I was able to connect and send HTTP requests to the IBM Tone Analyzer service to receive responses on the tone from a given news headline. This helped add multi-variation to the model by adding an extra column to the dataset for the model to improve from. However, the documentation provided additional information on using JSON to get data from JSON response objects, but the information is not relevant to my problem.

**F. Kotartemiy, K. (2020, June 30). GitHub - kotartemiy/pygooglenews: If Google News had a Python library. GitHub. Retrieved November 14, 2021, from https://github.com/kotartemiy/pygooglenews** - The Google News Python library documentation in the GitHub page for its repository, demonstrated how to install and use different methods from the library to get headlines. The main information that concerned my problem was the usage of the built-in search method used to receive a large number of news headlines. With the additional parameters for periods in the search method, I was able to search for headlines regarding Bitcoin between specific periods. The documentation contained several more methods and ways to create more search-specific headline lists, but I did not need that information for getting Bitcoin news headlines for tone analysis.

**G. M. (2020, November 22). GitHub - mrdbourke/tensorflow-deep-learning: All course materials for the zero to mastery deep learning with TensorFlow course. GitHub. Retrieved September 22, 2021, from https://github.com/mrdbourke/tensorflow-deep-learning** - The Tensorflow Deep Learning repository is for those who have participated in the Tensorflow Certification source. The GitHub repository contains Colab notebooks with theory and practical information on how to use Tensorflow. It specifically contained information about time-series problems, which allowed me to better shape my data to fit a time-series problem. I also utilized many important optimization methods, but the repository also includes information regarding projects, convolution, transfer learning, callbacks, natural language processing, classification models, and fundamental tensor modification. All of the information was relevant to my research excluding the majority of the information from the included natural language processing (NLP) notebooks used to create a project.

**H. Mueller, J. P., & Massaron, L. (2019). Deep Learning For Dummies (1st ed.) [E-book]. For Dummies.** - The Deep Learning For Dummies book by Mueller & Massaron demonstrates the fundamentals of both theory and practical ideas of Deep Learning. The book contains mathematical concepts such as matrices, vectors, and scalers. It also contains information regarding how to create and modify matrices using NumPy and Tensorflow. This information was the foundation of my background research as it helped me understand all the background processes that occur during a model's training and evaluation. However, I did not use the book to learn in-depth syntax as it was too detailed for my research timeframe. By understanding the basics of the Tensorflow library and Deep Learning, I could easily code a model while also being able to explain what the code executes.

**I. Zielak. (2021, April 11). Bitcoin Historical Data. Kaggle. Retrieved October 7, 2021, from https://www.kaggle.com/mczielinski/bitcoin-historical-data** - The Bitcoin Historical Data dataset available at Kaggle by Zielak contained a large dataset of Bitcoin prices with 1-minute intervals in Unix timestamps. The dataset timeframe was from Jan 2012 to March 2021 and contained columns with the volume, open price, close price, high price, low price, etc. I was able to utilize this dataset for the entire project because it had a large amount of data. However, I cut down the data's timeframe to start from December of 2015, and I also removed all columns except the open price and the Unix timestamps corresponding with the price. This dataset was therefore used throughout the entire project and served as a placeholder for the final dataset used to contain an extra column for tone data for multi-variation modeling.
