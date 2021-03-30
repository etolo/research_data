# Predicting financial crisis with recurrent neural networks

This file contains the program code behind the article Tölö, E., (2020). “Predicting financial crises with recurrent neural networks,” Journal of Financial Stability, Volume 49, August 2020, 100746. Available at: https://doi.org/10.1016/j.jfs.2020.100746.

This code is made available for advanced users. The code is designed such that it can be mostly (but not completely) run sequentially starting from the top.

First some libraries and data are imported. Then I define functions that transform the data (make it stationary, drop NaN values etc). Then more functions for the classification task, definition of models and model evaluation. After all the functions have been defined, the results are calculated by calling the function with specific input parameters - sometimes in a loop.

Some of the code is probably dense and hard to follow. That is mainly because of storing all the intermediate results and statistics for the article, and running all different options in a loop.

If you want to run some of the models included in the article, I recommend to extract the relevant parts of the code listed here, and build it into your own program.
 1. Data processing (top part of the code)
 2. Reshaping data to be suitable input to neural nets (search for reshape, there are one or two such short functions)
 3. Inspect getModel to find out how the neural net that you are interested can be initialized.
 4. Inspect fitModel to find out how the neural net that you are interested in can be fitted to the data.
 5. There are also functions for calculating the AUC statistics, usefulness, etc. that you may find useful.
 6. The cross-validation and sequential evaluation functions may also be of interest to you, albeit these parts of the code are somewhat complicated to read because of the factors mentioned earlier.
 7. There is also functions that implement the calculation and analysis of Shapley values. Feel free to use them, but may be easier (safer) to build your own.
 
**Cite as:**
 
**Tölö, E., (2020). “Predicting financial crises with recurrent neural networks,” Journal of Financial Stability, Volume 49, August 2020, 100746. Available at: https://doi.org/10.1016/j.jfs.2020.100746**