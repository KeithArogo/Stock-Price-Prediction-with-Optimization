# Stock-Price-Prediction-with-Optimization

About the Project.
Portfolio optimization is a process of allocating funds into financial assets with the goal of 
maximizing returns over risk. This research is our attempt at utilising machine learning methods to 
create an optimized portfolio that will perform well into the future. This was achieved by utilising 2
different Random Forest models to forecast stock prices, namely :
•Model 1 – uses technical indicator features.
•Model 2 – uses technical indicator features combined with sentiment features.
Having predicted the stock prices, we then calculate the relevant expected returns. From these we 
apply an optimisation technique, using a custom mean-variance loss function that optimises the 
returns over the portfolio risk. Each model repeats this process 500 times before proposing the best
suited portfolio as per the results.
Built With.
This section should list all the main packages used in the project.
•numpy
•pandas
•sklearn
•torch
•SciPy
•seaborn
•os
•matplotlib.pyplot
Methods and Concepts Used.
•Principal Component Analysis.
•Random Forest Regression.
•Optimisation.
Relevant Technologies.
•R
•Python
Getting Started.
The data set used in this project can be accessed and imported directly into each model, from the 
folder. The data pre-processing for each model is done in its respective Jupyter notebook. The 
suggested order to view the Jupyter notebooks begins with: 
1. Model 1.
2. Model 2.
3. Graphs.
Pre requirements.
•PyTorch 
Usage.
‘Model 1’ and ‘Model 2’ in the ‘Models’ folder, can be used to iteratively predict future stock prices
and optimize each the 5-asset portfolio’s weights depending on the results. The dataset expected is 
a 2d DataFrame, with dates as rows and different metrics for stocks in columns. These can be used
by simply running all cells in the notebook.
‘News extraction model’ demonstrates the extraction and manipulation of the said sentiment 
features (news headlines).
‘Comparison metrics’ takes results from ‘Model 1’ and ‘Model 2’ and displays graphs and visuals 
detailing their differences and similarities to draw conclusions
