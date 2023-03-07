# Final Project
## Project information
- **Author**: Runkun Guo, Applied Mathematics, 2023 , Duke Kunshan University
- **Instructor**: Prof. Luyao Zhang, Duke Kunshan University
- **Disclaimer**: Submissions to the Final Project for STATS201 Introduction to Machine Learning for Social Science, 2023 Spring Term (Seven Week - First) instructed by Prof. Luyao Zhang at Duke Kunshan University.
- **Acknowledgments**: Thanks to Professor Luyao Zhang for giving Inspiration to my project and the demo code she provides. Thanks for the support from every classmate of mine.
- **Project Summary**: 
  - Background: To predict the outcome of a certain soccer match may have a petential commercial value. We tried to find the correlation between the total number of shooting and the total number of goals in a match as a part of outcome of a match. Not many scholars are still doing research on this quite traditional gambling game theory. Thus, I want to make some improvements to this field.
  - Research Question: Does the eruption of COVID-19 have influence on the stock price of Zoom?
  - Data Source: I use the data of the stock price of Zoom queried from Zoom Inc. Official website.
  - Methods: I tried to use linear regression to predict the total numner of goals given a number of shooting and I also tried Ramdom forest Regression. Besides, I also consider the number of goals as a group of classes and I use Decision Tree Classifier to get the confusion matrix.
  - Results: The Stock price had a remarkable rise in the Date number 215 which is 03/03/2020 in the real world and it is also the week after the carry out of the online working and studying policy. The highest increment ratio reached 13.38 percent. Besides, there is also a tremendous drop in the stock price on 03/01/2022 by which time, COVID-19 got little influence on people's daily life and everything got normal like before the pandemic.
The accuracy of the Random Forest Classifier is 51% while the accuracy of the Multi-layer Classifier is 49%. The Random Forest Classifier seems to be a more appropriate Classifier for this question.
  - Intellectual Merits: The pandemic created a highly volatile market environment, and sentiment among investors can play a significant role in driving stock prices. Besides the normal monitoring key indicators such as trading volume, short interest, and institutional ownership provide insights into how investors viewed Zoom during the pandemic, the policy and new rules brought by the pandemic also influenced the stock's price.

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

## Poster
[Final Poster.pdf](https://github.com/Rising-Stars-by-Sunshine/stats201-Finalproject-Runkun_Guo/files/10909121/Final.Poster.pdf)


## Spotlight
<img width="1073" alt="截屏2023-02-26 下午9 30 23" src="https://user-images.githubusercontent.com/99957590/223415978-57312936-8380-4752-b3f2-200be9bce1ed.png">
Assumption: The uncommercial factors besides the occurrence of COVID-19 have little influence on the stock price of Zoom.

<img width="549" alt="截屏2023-03-07 下午8 06 51" src="https://user-images.githubusercontent.com/99957590/223417902-36a6cab1-612d-4932-b29e-c8b39944de0b.png">

<img width="973" alt="截屏2023-03-07 下午8 06 39" src="https://user-images.githubusercontent.com/99957590/223417934-825e8f47-533d-413b-9fab-eb0155954dde.png">

<img width="561" alt="截屏2023-03-07 下午8 06 17" src="https://user-images.githubusercontent.com/99957590/223417948-d88e2138-d6c6-40d9-af99-af026d38a3ac.png">

<img width="977" alt="截屏2023-03-07 下午8 06 05" src="https://user-images.githubusercontent.com/99957590/223417966-0f3b6d0e-f612-430b-94fe-7f0aaab43e13.png">


This Figure is the confusion matrix under Decision Tree. We can see that only few classes have a relatively strong correlation. 
<img width="731" alt="截屏2023-03-07 下午4 19 00" src="https://user-images.githubusercontent.com/99957590/223415786-2c748f09-926d-41fe-80ef-b438cba0c98f.png">


## References

### Data Source
[Zoom Inc. official website](https://investors.zoom.us/stock-information/stock-quote-chart/)
### Code Source
[Luyao Zhang's Sample Code](https://github.com/Rising-Stars-by-Sunshine/stats201-tutorial-prediction)

### Articles

Arora, N., & Kumari, A. (2021). Impact of COVID-19 on the Stock Prices of Zoom Video Communications. Journal of Finance and Economics Research, 6(1), 39-46.

Garg, D., Dutt, S., & Chandra, S. (2021). Analyzing the Impact of COVID-19 on Zoom Video Communications Stock Prices. Journal of Investment Strategies, 10(1), 41-50.

### Literature
Zhang, Luyao (Sunshine). 2022. “Machine Learning for Predictions.” Machine Learning for Social Science, November. https://ms.pubpub.org/pub/ml-prediction/release/4.

