# Final Project
## Project information
- **Author**: Runkun Guo, Applied Mathematics, 2023 , Duke Kunshan University
- **Instructor**: Prof. Luyao Zhang, Duke Kunshan University
- **Disclaimer**: Submissions to the Final Project for STATS201 Introduction to Machine Learning for Social Science, 2023 Spring Term (Seven Week - First) instructed by Prof. Luyao Zhang at Duke Kunshan University.
- **Acknowledgments**: Thanks to Professor Luyao Zhang for giving Inspiration to my project and the demo code she provides. Thanks for the support from every classmate of mine.
- **Project Summary**: 
  - Background: To predict the outcome of a certain soccer match may have a petential commercial value. We tried to find the correlation between the total number of shooting and the total number of goals in a match as a part of outcome of a match. Not many scholars are still doing research on this quite traditional gambling game theory. Thus, I want to make some improvements to this field.
  - Research Question: Does the number of shootings has correlation with the number of goals in a certain soccer match?
  - Data Source: I use the data queried from football.data.co.uk website which is a gambling website that records all the historical data for football matches in UK
  - Methods: I tried to use linear regression to predict the total numner of goals given a number of shooting and I also tried Ramdom forest Regression. Besides, I also consider the number of goals as a group of classes and I use Decision Tree Classifier to get the confusion matrix.
  - Results: From the Regression part, I found out that the accuracy of Random Forest Regression is only 19.49%. For the decision tree classification, the accuracy of f1 score is 22%. I may conclude that there's no direct or few connection between the total number of shooting and the number of goals.
  - Intellectual Merits: The result is quite opposite to my expectation that this two variables have few connections. In the beginging, I found out that the accuracy of regression is not very high, thus I try to make the discrete number as different classes and use the Decision Tree Classifier to make a prediction. However, the accuracy is still ideal enough. Therefore, based on my simulation resultes, I could only conclude my X and Y have few connections now. In the future, I may try to make my data more suitable for the models and may try to consider the discrete number into one-hot code for classification part to improve the accuracy

## Table of Contents
- [Data](https://github.com/Rising-Stars-by-Sunshine/stats201-PS2-Runkun_Guo/tree/main/data)
- [Code](https://github.com/Rising-Stars-by-Sunshine/stats201-PS2-Runkun_Guo/tree/main/Code)
- [Spotlight](https://github.com/Rising-Stars-by-Sunshine/stats201-PS2-Runkun_Guo/tree/main/spotlight)


## Data
|Data Files                   | Data Content                                             | Data Type                                       | 
|:---      |   :---:     |     ---:|
|E0.csv&E1.csv|Historical data from the data website | Queried data |
|[Queried Data](https://github.com/Rising-Stars-by-Sunshine/stats201-PS2-Runkun_Guo/blob/main/data/E0.csv)| Data after merging and selecting| Processed data|
|[Processed Data](https://github.com/Rising-Stars-by-Sunshine/stats201-PS2-Runkun_Guo/tree/main/data/Data)| Data after spliting for training and testing|Processed data |

## Data Dictionary
|Variable Name    | Description     | Frequency      | Unit    | Range      | Type        |
|:---      |   :---:     |     ---:|    ---:|    ---:|    ---:|
|MatchTime | When the match occurs | Daily | Hour | Two match seasons |  Time     |
|Total Shooting| The total number of shootings | Discrete   | Number   | 9-53   | Integer   |
|Total Score   | The total number of goals     | Discrete   | Number   | 0-9    | Integer   |


## Code
- [Query Data](https://github.com/Rising-Stars-by-Sunshine/stats201-PS2-Runkun_Guo/blob/main/Code/Query_Data_Runkun_Guo.ipynb)
- [Process Data](https://github.com/Rising-Stars-by-Sunshine/stats201-PS2-Runkun_Guo/blob/main/Code/Process_Data_PrepareX%26Y_Variable_Runkun_Guo.ipynb)
- [Analyze Data](https://github.com/Rising-Stars-by-Sunshine/stats201-PS2-Runkun_Guo/blob/main/Code/“Analyze_Data_Predicting_Runkun_Guo_ipynb”.ipynb)

## Spotlight
<img width="607" alt="Linear Regression" src="https://user-images.githubusercontent.com/99957590/219958742-ba824161-dab4-40f6-b729-cf0900894a7e.png">
This figure is the prediction distribution under Linear Regression. It's obvious that the regression is not very ideal.
<img width="542" alt="Random Forest" src="https://user-images.githubusercontent.com/99957590/219958863-f8c3ee77-e063-454a-9fcb-8e831eca2792.png">
This figure is the prediction distribution under Random Forest. 
<img width="503" alt="Decision Tree correlation" src="https://user-images.githubusercontent.com/99957590/219958872-ba56cf01-dd29-486f-bb52-43f2cb5ded80.png">
This Figure is the confusion matrix under Decision Tree. We can see that only few classes have a relatively strong correlation. 
<img width="731" alt="截屏2023-03-07 下午4 19 00" src="https://user-images.githubusercontent.com/99957590/223415786-2c748f09-926d-41fe-80ef-b438cba0c98f.png">

## References

### Data Source
[Football data UK](https://www.football-data.co.uk/data.php)
### Code Source
[Luyao Zhang's Sample Code](https://github.com/Rising-Stars-by-Sunshine/stats201-tutorial-prediction)

### Articles


[Saritha, M., Milton, R.S. RETRACTED ARTICLE: A probabilistic logic approach to outcome prediction in team games using historical data and domain knowledge. J Ambient Intell Human Comput 12, 5205–5214 (2021).](https://doi-org.proxy.lib.duke.edu/10.1007/s12652-020-01989-x)

### Literature
Zhang, Luyao (Sunshine). 2022. “Machine Learning for Predictions.” Machine Learning for Social Science, November. https://ms.pubpub.org/pub/ml-prediction/release/4.

