# Final Project
## General information
- **Author**: Runkun Guo, Applied Mathematics, 2023 , Duke Kunshan University
- **Instructor**: Prof. Luyao Zhang, Duke Kunshan University
- **Disclaimer**: Submissions to the Final Project for STATS201 Introduction to Machine Learning for Social Science, 2023 Spring Term (Seven Week - First) instructed by Prof. Luyao Zhang at Duke Kunshan University.
- **Acknowledgments**: Thanks to Professor Luyao Zhang for giving Inspiration to my project and the demo code she provides. Thanks for the support from every classmate of mine.

## Project Summary
  - **Background & Motivation**: The COVID-19 pandemic is an extreme event that has brought uncertainty to the financial markets, led to a sudden fall in stock prices, and has given rise to financial volatility (Mahata et al., 2021). Many companies experienced fluctuations in their stock prices during the pandemic. One such company is Zoom Inc., a video communication software provider that saw a surge in demand as a result of online working and studying policy during the pandemic. This project will examine the effect that the pandemic had on Zoom Inc.'s stock price from 04/18/2019 to 02/24/2023 and explore the various factors like official policies that may contribute to these changes. By analyzing the impact of the pandemic on Zoom Inc.'s stock price, we can gain insights into the ways in which the pandemic has affected the business world and the stock market as a whole.
  - **Research Question**: Does the eruption of COVID-19 have influence on the stock price of Zoom?
  - **Data Source**: The data of the stock price of Zoom is directly queried from Zoom Inc. Official website. The data is from 04/18/2019 to 02/24/2023.
  - **Methods**: The researcher applies a grest number of machine learning algorithms to both prediction and casual inference part. The linear regression and random forest regression are applied to predict the future trend of changing of the stock price. Random forest classifier is also applied to find out if the trend of changing is correlated with the past data. For the casual inference part, a figure with a prediction is drew with Visual Workspace 2023, proposing the hypotheses about the occruance of the pandemic had positive influence on the stock price. Then, with Scikit-learn Regression tool, a graph is provided to visualize the influence of the pandemic on the stock price.
  - **Results**: The Stock price had a remarkable rise in the Date number 215 which is 03/03/2020 in the real world and it is also the week after the carry out of the online working and studying policy. The highest increment ratio reached 13.38 percent. Besides, there is also a tremendous drop in the stock price on 03/01/2022 by which time, COVID-19 got little influence on people's daily life and everything got normal like before the pandemic.
The accuracy of the Random Forest Classifier is 51% while the accuracy of the Multi-layer Classifier is 49%. The Random Forest Classifier seems to be a more appropriate Classifier for this question.
  - **Intellectual Merits**: The pandemic created a highly volatile market environment, and sentiment among investors can play a significant role in driving stock prices. Besides the normal monitoring key indicators such as trading volume, short interest, and institutional ownership provide insights into how investors viewed Zoom during the pandemic, the policy and new rules brought by the pandemic also influenced the stock's price.

## Table of Contents
- [Data](https://github.com/Rising-Stars-by-Sunshine/stats201-PS2-Runkun_Guo/tree/main/data)
- [Code](https://github.com/Rising-Stars-by-Sunshine/stats201-PS2-Runkun_Guo/tree/main/Code)
- [Spotlight](https://github.com/Rising-Stars-by-Sunshine/stats201-PS2-Runkun_Guo/tree/main/spotlight)
- [More about the Author]
- - [References]

## Meta Data Information
|Data Files                   | Data Content                                             | Data Type                                       | 
|:---      |   :---:     |     ---:|
|[ZoomData.csv](https://github.com/Rising-Stars-by-Sunshine/stats201-Finalproject-Runkun_Guo/blob/main/data/Data/ZoomData.csv)|Historical stock price data from the data website | Queried data |
|[Regression_Train.csv](https://github.com/Rising-Stars-by-Sunshine/stats201-Finalproject-Runkun_Guo/blob/main/data/Data/Regression_Train.csv)| Training data for Regression| Processed data|
|[Regression_Test.csv](https://github.com/Rising-Stars-by-Sunshine/stats201-Finalproject-Runkun_Guo/blob/main/data/Data/Regression_Test.csv)| Test data for Regression|Processed data |
|[Classification_Train.csv](https://github.com/Rising-Stars-by-Sunshine/stats201-Finalproject-Runkun_Guo/blob/main/data/Data/Classification_Train.csv)| Training data for Classification|Processed data |
|[Classification_Test.csv](https://github.com/Rising-Stars-by-Sunshine/stats201-Finalproject-Runkun_Guo/blob/main/data/Data/Classification_Test.csv)|Test data for Classification|Processed data |
|[final.csv](https://github.com/Rising-Stars-by-Sunshine/stats201-Finalproject-Runkun_Guo/blob/main/data/Data/final.csv)| Related journals' title and abstract | Queried data|


## Data Dictionary
|File Name |Variable Name    | Description     | Frequency      | Unit    | Range      | Type        |
|:---     |   :---:      |   :---:     |     ---:|    ---:|    ---:|    ---:|
|ZoomData.csv |Date | Trading day in a year | Daily | Day | 4/18/2019 to 2/24/2023|  Time     |
|             |Close Price| Close Price of the stock every day| Daily | USD$  |  4/18/2019 to 2/24/2023| Float |
|Regression_Train.csv|  ROI | The trend and degree of changing   | None | None   | None  | Float |
|             |Unnamed Date | Trading day in a year with number | Daily | th | 0-628 |  Integer    |
|Regression_Test.csv  |  ROI | The trend and degree of changing   | None | None   | None  | Float |
|             |Unnamed Date | Trading day in a year with number | Daily | th | 628-942 |  Integer    |
|Classification_Train.csv  |  Positive | The trend of changing (label) | None | None   | None  | 1/0 |
|             |ROI_past_ma10 | The trend of changing in the past 10 days | Daily | None | 0-628 |  Float    |
|Classification_Test.csv  |  Positive | The trend of changing (label) | None | None   | None  | 1/0 |
|             |ROI_past_ma10 | The trend of changing in the past 10 days | Daily | None | 628-942 |  Float |
|final.csv  |  Title| Titles of 7 related journals | None | None   | None  | str |
|             |Abstract| Abstracts of 7 related journals| None | None | 628-942 |  str |

## Code
- [Query Data](https://github.com/Rising-Stars-by-Sunshine/stats201-PS2-Runkun_Guo/blob/main/Code/Query_Data_Runkun_Guo.ipynb)
- [Process Data](https://github.com/Rising-Stars-by-Sunshine/stats201-PS2-Runkun_Guo/blob/main/Code/Process_Data_PrepareX%26Y_Variable_Runkun_Guo.ipynb)
- [Analyze Data](https://github.com/Rising-Stars-by-Sunshine/stats201-PS2-Runkun_Guo/blob/main/Code/“Analyze_Data_Predicting_Runkun_Guo_ipynb”.ipynb)

## Poster
[Final Poster.pdf](https://github.com/Rising-Stars-by-Sunshine/stats201-Finalproject-Runkun_Guo/files/10909121/Final.Poster.pdf)

![Final Poster](https://user-images.githubusercontent.com/99957590/223969938-35361c2d-51e8-4580-8c39-a67572036dc6.png)

Figure NO.1. Final Project Poster

An illustrated poster in Figure No.1. briefly describes the research project. Contents include: Abstract, Background, Methodology, Result, Conclusion, References, and Acknowledgement. Created in [Canva](https://www.canva.com/zh_cn/).

## Spotlight
<img width="1073" alt="截屏2023-02-26 下午9 30 23" src="https://user-images.githubusercontent.com/99957590/223415978-57312936-8380-4752-b3f2-200be9bce1ed.png">
Figure NO.2. Causal Inference research design

Figure NO.2. demonstrates the casual inference design for the influence brought by the eruption of COVID-19 on the stock price of Zoom aspect to the stock price. The outbreak of the COVID-19 pandemic in 2020 has had a profound impact on the global economy, including the stock market. One company that experienced significant changes in its stock price during this time was Zoom Video Communications, Inc. The Covid-19 pandemic has not only changed the mode of study and work from face-to-face (offline) to online, but also affects business/economic activities in terms of decreasing profits and decreasing economic growth.(Putri et al., 2022) The Zoom Inc. saw the increasing demand of online communication APP. As a result, the stock price of Zoom Video spiked more than 100% since January as coronavirus pushes millions to work from home. From this historical data, there's no denying that the eruption of COVID-19 and the policy of remote working and studying had positive influence on the stock price of Zoom. This study will use the regression discontinuity algorithm to research " Does the eruption of COVID-19 have influence on the stock price of Zoom?" The research is based on the assumption that: The uncommercial factors besides the occurrence of COVID-19 have little influence on the stock price of Zoom. The hypothesis is: The occurrence of COVID-19 has a positive local average treatment effect on the stock price. 

![Unknown](https://user-images.githubusercontent.com/99957590/223867265-fa121948-394b-43f6-873c-0d83104612f9.png)
Figure NO.3. " Pandemic Impact" journal titles' word cloud

By searching a number of relative journals about the influence of the pandemic on the Zoom stock price, a word cloud is generated by NLP. For the titles, it is obvious that the word "COVID" , "Pandemic" and " Impact" have the highest frequency of appearance. This indicates that our research question may have some references to support.
![Unknown-2](https://user-images.githubusercontent.com/99957590/223867321-044e8fba-7930-4e0c-8df6-16c55ca07197.png)
Figure NO.4. " Pandemic Impact" journal abstract' word cloud

By searching a number of relative journals about the influence of the pandemic on the Zoom stock price, a word cloud is generated by NLP. For the abstracts, the words " Women ", " COVID " and " Students " have the highest frequency of appearance. The following research may find out the correlation between them.

<img width="549" alt="截屏2023-03-07 下午8 06 51" src="https://user-images.githubusercontent.com/99957590/223417902-36a6cab1-612d-4932-b29e-c8b39944de0b.png">
Figure NO.5. Linear Regression prediction histogram of Stock Price 

<img width="973" alt="截屏2023-03-07 下午8 06 39" src="https://user-images.githubusercontent.com/99957590/223417934-825e8f47-533d-413b-9fab-eb0155954dde.png">
Figure NO.6. Linear Regression prediction line graph of changing trend

Figure NO.5. illustrates the prediction of the stock price made by linear regression, where the blue part represents the real data and the green part represents the data predicted by linear regression. It can be concluded from the graph that the prediction result is not very ideal with an accuracy of 0.05%, and it may due to the choice of the regression model and the pre-processing of data. The centralized of prediction result may due to the centralized norm of input and in the real world, stock price may not change in the linear way.
Figure NO.6. shows the prediction of the changing trend made by linear regressin. If the value of y-axis is positive then it implies the stock price rises， vice versa.  The x-axis represents the day of stock trading counted in numbers. The linear prediction line does not fit the actual curve of changing very well. This result may explain the low accuracy of prediction of this model that linear regression is not the best model for the prediction of stock changing trend. 

<img width="561" alt="截屏2023-03-07 下午8 06 17" src="https://user-images.githubusercontent.com/99957590/223417948-d88e2138-d6c6-40d9-af99-af026d38a3ac.png">
Figure NO.7. Random Forest prediction line graph of changing trend


<img width="977" alt="截屏2023-03-07 下午8 06 05" src="https://user-images.githubusercontent.com/99957590/223417966-0f3b6d0e-f612-430b-94fe-7f0aaab43e13.png">
Figure NO.8. Random Forest prediction line graph of changing trend



<img width="731" alt="截屏2023-03-07 下午4 19 00" src="https://user-images.githubusercontent.com/99957590/223415786-2c748f09-926d-41fe-80ef-b438cba0c98f.png">
Figure NO.9.

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

