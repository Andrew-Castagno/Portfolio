# Portfolio

#### Quick Guide
1. For Python and some SQL coding skills [click here](https://github.com/Andrew-Castagno/Portfolio/blob/main/Youtube%20API%20Pipeline%20-%20Full%20Thoughts.ipynb)
2. For R EDA and visualization skills [click here](https://github.com/Andrew-Castagno/Portfolio/blob/main/EDA-and-Visualization---Sentiment-Analysis.md)
3. For geospatial visualizations [click here](https://github.com/Andrew-Castagno/scholometrics/blob/main/Geospatial/Geospatial_aerosol_visualization.md)
4. For some modeling in R [click here](https://github.com/Andrew-Castagno/scholometrics/blob/main/SMOTE%20with%20GLM/SMOTE-with-GLM.md)



 
    
#### YouTube project:
## The Sky is Falling 
### The impact of title sentiment on the success of scientific YouTube content

The goal of this project is to gain insights into the impact of video title sentiment (positive, negative, or neutral) on the overall performance of the video for the popular science YouTube channel, Kurzgesagt.


### Outline
Each of the steps outlined below is a markdown file which explains my logic as I go through them. Therefore, I will only provide a light overview here.

##### 1. [Building a data pipeline and working with API's and AWS in Python](https://github.com/Andrew-Castagno/Portfolio/blob/main/Youtube%20API%20Pipeline%20-%20Full%20Thoughts.ipynb)

##### 2. [Performing EDA and crafting visualizations in R](https://github.com/Andrew-Castagno/Portfolio/blob/main/EDA-and-Visualization---Sentiment-Analysis.md)


### Core Insights

#### NLP Sentiment Analysis Model Insights
![model vs human comparison](https://github.com/Andrew-Castagno/Portfolio/blob/main/EDA-and-Visualization---Sentiment-Analysis_files/figure-gfm/model-comparison-barplot-1.png)

When comparing the sentiment analysis model to human-assigned title sentiments, an issue that was observed is that the sentiment analysis model tended towards assigning all titles to either "positive" or "negative" classifications, and would rarely assign titles a "neutral" classification. The distribution of positive and negative assignments, on the other hand, were similar between the human and model classifications. 

#### Comparison Between Sentiments for all Metrics
![All violins](https://github.com/Andrew-Castagno/Portfolio/blob/main/EDA-and-Visualization---Sentiment-Analysis_files/figure-gfm/violin-sentiment-plots-1.png)

Higher rates of engagement (likes and comments) were observed for both positive and negative titles than for neutral titles. However, only negative titles showed an increase in views over neutral titles (t-test p=.09). 

#### Comparison Between Sentiments for only Views
![views only violin](https://github.com/Andrew-Castagno/Portfolio/blob/main/EDA-and-Visualization---Sentiment-Analysis_files/figure-gfm/views-violin-plot-1.png)

Looking at views more closely, the higher median view count in negative videos is apparent (here outliers have been removed). 

#### Timeseries of Metrics
![timeseries](https://github.com/Andrew-Castagno/Portfolio/blob/main/EDA-and-Visualization---Sentiment-Analysis_files/figure-gfm/timeseries-1.png)

While engagement metrics (likes and comments) have increased over time, views have remained constant. The likely explanation is that new viewers will comment and like on the new videos that they engage with, but as they go back through the backlog to view older videos they do not leave likes or comments.


### Future Goals

Future iterations of this project will be built out to incorporate multiple YouTube channels, first from popular science and then from additional video genres with a long-term goal of creating a tool which can suggest optimal titles based on the topic and genre of a video along with keywords.
