# The Effect of the Pandemic to the Stock Price of Zoom
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
  - **Results**: The Zoom's stock price increased substantially during the early stages of the pandemic due to the sudden surge in remote work and online communication. However, Zoom's stock price declined to a pre-pandemic level as the pandemic progressed and vaccine rollouts began.
  - **Intellectual Merits and Practical impacts**: 
  - ***Investment decisions*** This project provides investors and shareholders with a warning for future pandemics and such events.
  - ***Public health policy*** The research could have implications for public health policy by highlighting the economic impacts of pandemics. The findings could be used to inform policies aimed at mitigating the economic impact of pandemics, such as stimulus packages and financial support for affected companies.
  - ***Business strategy*** Zoom Inc. and other companies could use the research findings to develop effective strategies to respond to the challenges posed by pandemics. The research would provide insights into the factors that influence investor behavior during pandemics and how companies can respond to these factors.
  - ***Advancing knowledge*** This research would add to the existing body of knowledge about the impact of pandemics on the stock prices of companies. It would provide insights into the dynamics of the stock market during pandemics and how specific companies, such as Zoom Inc., are affected.

## Table of Contents
- [Data](https://github.com/Rising-Stars-by-Sunshine/stats201-PS2-Runkun_Guo/tree/main/data)
- [Code](https://github.com/Rising-Stars-by-Sunshine/stats201-PS2-Runkun_Guo/tree/main/Code)
- [Spotlight](https://github.com/Rising-Stars-by-Sunshine/stats201-PS2-Runkun_Guo/tree/main/spotlight)
- [More about the Author](https://github.com/Rising-Stars-by-Sunshine/stats201-Finalproject-Runkun_Guo#More-about-the-Author)
- [References](https://github.com/Rising-Stars-by-Sunshine/stats201-Finalproject-Runkun_Guo#References)

## Meta Data Information
|Data Files                   | Data Content                                             | Data Type                                       | 
|:---      |   :---:     |     ---:|
|[ZoomData.csv](https://github.com/Rising-Stars-by-Sunshine/stats201-Finalproject-Runkun_Guo/blob/main/data/Data/ZoomData.csv)|Historical stock price data from the data website | Queried data |
|[Regression_Train.csv](https://github.com/Rising-Stars-by-Sunshine/stats201-Finalproject-Runkun_Guo/blob/main/data/Data/Regression_Train.csv)| Training data for Regression| Processed data|
|[Regression_Test.csv](https://github.com/Rising-Stars-by-Sunshine/stats201-Finalproject-Runkun_Guo/blob/main/data/Data/Regression_Test.csv)| Test data for Regression|Processed data |
|[Classification_Train.csv](https://github.com/Rising-Stars-by-Sunshine/stats201-Finalproject-Runkun_Guo/blob/main/data/Data/Classification_Train.csv)| Training data for Classification|Processed data |
|[Classification_Test.csv](https://github.com/Rising-Stars-by-Sunshine/stats201-Finalproject-Runkun_Guo/blob/main/data/Data/Classification_Test.csv)|Test data for Classification|Processed data |
|[final.csv](https://github.com/Rising-Stars-by-Sunshine/stats201-Finalproject-Runkun_Guo/blob/main/data/Data/final.csv)| Related journals' title and abstract | Queried data|

### Data Source
[Zoom Inc. official website](https://investors.zoom.us/stock-information/stock-quote-chart/)


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
- [Process Data](https://github.com/Rising-Stars-by-Sunshine/stats201-Finalproject-Runkun_Guo/blob/main/Code/“Process_Code__ipynb_Runkun_Guo”.ipynb)
- [Analyze Data](https://github.com/Rising-Stars-by-Sunshine/stats201-Finalproject-Runkun_Guo/blob/main/Code/“Analyze_Data_ipynb_Runkun_Guo”.ipynb)
- [Casual Inference](https://github.com/Rising-Stars-by-Sunshine/stats201-Finalproject-Runkun_Guo/blob/main/Code/Final_Causual.ipynb)
- [Word Cloud](https://github.com/Rising-Stars-by-Sunshine/stats201-Finalproject-Runkun_Guo/blob/main/Code/“NLP_Blockchain.ipynb)

## Table of Code

<div class="table-wrapper" markdown="block">
 
| Code files| Description | Type| Task|
| :---         |     :---     | :--- | :---|
| [“NLP_Blockchain.ipynb](https://github.com/Rising-Stars-by-Sunshine/stats201-Finalproject-Runkun_Guo/blob/main/Code/“NLP_Blockchain.ipynb) |Code using the NLP method to generate word cloud and bigram | .ipynb | Explanation| 
| [“Process_Code__ipynb_Runkun_Guo”.ipynb](https://github.com/Rising-Stars-by-Sunshine/stats201-Finalproject-Runkun_Guo/blob/main/Code/“Process_Code__ipynb_Runkun_Guo”.ipynb) | Code processing the X and Y dataset from Ethereum_value.csv for regression  | .ipynb | Prediction| 
| [“Analyze_Data_ipynb_Runkun_Guo”.ipynb](https://github.com/Rising-Stars-by-Sunshine/stats201-Finalproject-Runkun_Guo/blob/main/Code/“Analyze_Data_ipynb_Runkun_Guo”.ipynb) | Code applying machine learning method for open price regression| .ipynb | Prediction | 
| [Final_Causual.ipynb](https://github.com/Rising-Stars-by-Sunshine/stats201-Finalproject-Runkun_Guo/blob/main/Code/Final_Causual.ipynb) | Code applying the regression discontinuity method | .ipynb | Causal Inference| 
 
 </div>

## Poster
[Final Poster.pdf](https://github.com/Rising-Stars-by-Sunshine/stats201-Finalproject-Runkun_Guo/files/10909121/Final.Poster.pdf)

![Final Poster](https://user-images.githubusercontent.com/99957590/223969938-35361c2d-51e8-4580-8c39-a67572036dc6.png)

Figure NO.1. Final Project Poster

An illustrated poster in Figure No.1. briefly describes the research project. Contents include: Abstract, Background, Methodology, Result, Conclusion, References, and Acknowledgement. Created in [Canva](https://www.canva.com/zh_cn/).

## Spotlight
<img width="1073" alt="截屏2023-02-26 下午9 30 23" src="https://user-images.githubusercontent.com/99957590/223415978-57312936-8380-4752-b3f2-200be9bce1ed.png">
Figure NO.2. Causal Inference research design

Figure NO.2. demonstrates the casual inference design for the influence brought by the eruption of COVID-19 on the stock price of Zoom aspect to the stock price. The outbreak of the COVID-19 pandemic in 2020 has had a profound impact on the global economy, including the stock market. One company that experienced significant changes in its stock price during this time was Zoom Video Communications, Inc. The Covid-19 pandemic has not only changed the mode of study and work from face-to-face (offline) to online, but also affects business/economic activities in terms of decreasing profits and decreasing economic growth.(Putri et al., 2022) The Zoom Inc. saw the increasing demand of online communication APP. As a result, the stock price of Zoom Video spiked more than 100% since January as coronavirus pushes millions to work from home. From this historical data, there's no denying that the eruption of COVID-19 and the policy of remote working and studying had positive influence on the stock price of Zoom. This study will use the regression discontinuity algorithm to research " Does the eruption of COVID-19 have influence on the stock price of Zoom?" The research is based on the assumption that: The uncommercial factors besides the occurrence of COVID-19 have little influence on the stock price of Zoom. The hypothesis is: The occurrence of COVID-19 has a positive local average treatment effect on the stock price. 

Created by [Whimsical](https://whimsical.com/everyone-in-workspace-UHatk4cdJ4vgXf6G3kv3ry)

![Unknown](https://user-images.githubusercontent.com/99957590/223867265-fa121948-394b-43f6-873c-0d83104612f9.png)
Figure NO.3. " Pandemic Impact" journal titles' word cloud

By searching a number of relative journals about the influence of the pandemic on the Zoom stock price, a word cloud is generated by NLP. For the titles, it is obvious that the word "COVID" , "Pandemic" and " Impact" have the highest frequency of appearance. This indicates that our research question may have some references to support.
![Unknown-2](https://user-images.githubusercontent.com/99957590/223867321-044e8fba-7930-4e0c-8df6-16c55ca07197.png)
Figure NO.4. " Pandemic Impact" journal abstract' word cloud

By searching a number of relative journals about the influence of the pandemic on the Zoom stock price, a word cloud is generated by NLP. For the abstracts, the words " Women ", " COVID " and " Students " have the highest frequency of appearance. The following research may find out the correlation between them.

Created by [Blockchain Related SoKs](https://github.com/sunshineluyao/design-principle-blockchain)

<img width="549" alt="截屏2023-03-07 下午8 06 51" src="https://user-images.githubusercontent.com/99957590/223417902-36a6cab1-612d-4932-b29e-c8b39944de0b.png">
Figure NO.5. Linear Regression prediction histogram of Stock Price 

<img width="973" alt="截屏2023-03-07 下午8 06 39" src="https://user-images.githubusercontent.com/99957590/223417934-825e8f47-533d-413b-9fab-eb0155954dde.png">
Figure NO.6. Linear Regression prediction line graph of changing trend

Figure NO.5. illustrates the prediction of the stock price made by linear regression, where the blue part represents the real data and the green part represents the data predicted by linear regression. It can be concluded from the graph that the prediction result is not very ideal with an accuracy of 0.05%, and it may due to the choice of the regression model and the pre-processing of data. The centralized of prediction result may due to the centralized norm of input and in the real world, stock price may not change in the linear way.

Figure NO.6. shows the prediction of the changing trend made by linear regression. If the value of y-axis is positive then it implies the stock price rises， vice versa.  The x-axis represents the day of stock trading counted in numbers. The linear prediction line does not fit the actual curve of changing very well. This result may explain the low accuracy of prediction of this model that linear regression is not the best model for the prediction of stock changing trend. 

Supported by [Prof. Zhang's code for prediction](https://github.com/Rising-Stars-by-Sunshine/stats201-tutorial-prediction/blob/main/code/Analyze_Data_Machine_Learning_for_Predicting_Market_Congestion.ipynb)

<img width="561" alt="截屏2023-03-07 下午8 06 17" src="https://user-images.githubusercontent.com/99957590/223417948-d88e2138-d6c6-40d9-af99-af026d38a3ac.png">
Figure NO.7. Random Forest prediction line graph of changing trend

Figure NO.7. illustrates the prediction of the stock price made by Random Forest regression, where the blue part represents the real data and the green part represents the data predicted by linear regression. From the figure, the green bars matching the blue bars more than the linear regression with an accuracy of 49.8%. Compared to the linear regression, it could be concluded that random forest is more fitting of prediction than linear regression.

<img width="977" alt="截屏2023-03-07 下午8 06 05" src="https://user-images.githubusercontent.com/99957590/223417966-0f3b6d0e-f612-430b-94fe-7f0aaab43e13.png">
Figure NO.8. Random Forest prediction line graph of changing trend

Figure NO.8. shows the prediction of the changing trend made by Random Forest regression. If the value of y-axis is positive then it implies the stock price rises， vice versa.  The x-axis represents the day of stock trading counted in numbers. This time the prediction curve fits the test curve quite closely. Moreover, the yellow vertical line represents the highest rate of rising of the stock price and it happened on March 3rd, 2020. The black vertical line represents the highest rate of decreasing of the stock price and it happened on March 1st, 2022. This two dates will be used for the following causal inference part, and reasons will be given there.


<img width="731" alt="截屏2023-03-07 下午4 19 00" src="https://user-images.githubusercontent.com/99957590/223415786-2c748f09-926d-41fe-80ef-b438cba0c98f.png">
Figure NO.9. Causal Inference Result 

Figure NO.9. shows the close price of Zoom stock from 04/18/2019 to 02/24/2023, where the red and blue vertical lines represent the date when the stock price had the highest rate of rising or decreasing founded in the last part. The left orange line represents the original fitted line of the stock close price before the cut-off event happened on March 3rd, 2020. According to CNN News, "In March 2020, companies across the US abruptly shuttered their offices and instructed employees to work from home indefinitely as a result of the pandemic." (CNN, 2021) The remote working and studying policy in March 2020 was the cut-off event for the discontinuity of the stock price. Since then, the stock price kept rising until the beginning of 2021. The online-working a & studying policy due to the pandemic indeed brought increasement to the Zoom Stock price. The Hypothesis was tested. Furthermore, the decreasing green line is the fitted line after March 1st, 2022, when the stock price fell to the same level as it was before the cut-off event. The blue vertical line is also a causal event as the pandemic progressed and vaccine rollouts began. Everything went back to normal and the post-pandemic period came. The maroon fitted line between these two cut-off events is almost horizontal due to the stock price fellt o the same level as it was before March 2020. Overall, the pandemic had both positive and negative effects on Zoom's stock price, highlighting the complex nature of the stock market during a crisis. 

Supported by [numpy.polyfit](https://numpy.org/doc/stable/reference/generated/numpy.polyfit.html)


### AI Ethics Issues 
There is the potential for AI systems to be used for malicious purposes during a pandemic. For example, an AI system could be used to manipulate stock prices by spreading false information about a company's ability to handle the pandemic. This could lead to significant financial losses for investors and could damage the reputation of the targeted company.

### Future Work
This project only reveal the superficial correlation between the Pandemic and the stock price. In the future, the influence of actions and policies made by companies and government should be quantized and analyzed with more advanced analytical tools. In that way, the potential effect of these measurements maybe divinable so that the global financial market keeps in a stable and autonomous situation for developing.


## More about the Author
* Self Introduction

Runkun Guo, a senior majoring in Applied Mathematics and Computational Science at Duke Kunshan University. 

Field of research: Image compression based on SVD & Automatic detection of cancer tissues images based on CNN

![IMG_7010](https://user-images.githubusercontent.com/99957590/224016014-468de9e5-681d-48f4-b6c3-d14fd521d26a.JPG)

* Final Reflections:

Intellectual growth: This course typically covers the fundamental principles and techniques of statistics as applied to social science research. Over time, this course has evolved to reflect changes in both statistical methods and the research questions being studied in the social sciences. I have learnt the methods to deal with real-world social science issues with my statistics background.

Professional growth: This course can provide me with a foundation in statistical analysis and data interpretation, which can be useful in a variety of professional settings including: Data Analysis, Policy Development and Consulting. From my final project, I've learnt that statistics can be important in policy development, particularly in fields such as public health, social work, and criminal justice. Individuals with a background in statistics can help develop evidence-based policies and analyze the impact of those policies.

Living a purposeful life: After having this course, I could focus more on machine learning methods and causal inference that may be applied to a certain phenomena. I will also start to learn more analytical tools for solving social science issues that I'm interested in.

## References

### Data Source
[Zoom Inc. official website](https://investors.zoom.us/stock-information/stock-quote-chart/)

### Code Source
Prediction:[Luyao Zhang's Sample Code](https://github.com/Rising-Stars-by-Sunshine/stats201-tutorial-prediction)

Causal Event:[Python numpy.polyfit](https://numpy.org/doc/stable/reference/generated/numpy.polyfit.html)

Explaination: [Luyao Zhang's Sample Code](https://github.com/sunshineluyao/design-principle-blockchain)


### Articles

Arora, N., & Kumari, A. (2021). Impact of COVID-19 on the Stock Prices of Zoom Video Communications. Journal of Finance and Economics Research, 6(1), 39-46.

Aristovnik, Aleksander, Damijana Keržič, Dejan Ravšelj, Nina Tomaževič, and Lan Umek. 2020. "Impacts of the COVID-19 Pandemic on Life of Higher Education Students: A Global Perspective" Sustainability 12, no. 20: 8438. https://doi.org/10.3390/su12208438

Garg, D., Dutt, S., & Chandra, S. (2021). Analyzing the Impact of COVID-19 on Zoom Video Communications Stock Prices. Journal of Investment Strategies, 10(1), 41-50.

Kordestani, A., Pashkevich, N., Oghazi, P., Sahamkhadam, M., Sohrabpour, V. (2022) Effects of the COVID-19 pandemic on stock price performance of blockchain-based companies
Ekonomska Istrazivanja, 35(1): 3206-3224 https://doi.org/10.1080/1331677X.2021.1986676

Mahata, A., Rai, A., Nurujjaman, M., Prakash, O., & Prasad Bal, D. (2021). Characteristics of 2020 stock market crash: The COVID-19-induced extreme event. Chaos: An Interdisciplinary Journal of Nonlinear Science, 31(5), 053115. https://doi.org/10.1063/5. 0046704 

Noramalina A., Nur H., Intan A. (2022) Impact of COVID-19 Pandemic in Malaysia: A Critical Survey.  SOCIAL SCIENCES & HUMANITIES , 30 (4).  http://www.pertanika.upm.edu.my/



### Literature
Zhang, Luyao (Sunshine). 2022. “Machine Learning for Predictions.” Machine Learning for Social Science, November. https://ms.pubpub.org/pub/ml-prediction/release/4.

[CNN News. 2021.](https://edition.cnn.com/2021/03/09/success/remote-work-covid-pandemic-one-year-later/index.html)
