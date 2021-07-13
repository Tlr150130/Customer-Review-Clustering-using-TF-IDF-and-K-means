# Customer-Review-Clustering-using-TF-IDF-and-K-means
One of the greatest assets for the continuous improvement of a business is customer reviews. For example, reviews can help acknowledge the successes of the business while illuminating areas of potential development. The task is easy when there are few reviews. However, when there are many reviews and many more continuously being submitted, this becomes a seemingly insurmountable task. This is where automation and machine learning is crucial.

Our goal for this project is to take all reviews available on yelp and cluster them into like-minded groups. From there, we will condense their reviews into significant information for quick analysis. Using the significant information, the most impactful issues are highlighted and business improvement plans can be developed.

Here we will utilize BeautifulSoup's webscraping capabilities to gather all reviews for subsequent analysis. The reviews will be preprocessed to reduce noise within the data. The processed data will be converted to comparable numerical quantities using the TF-IDF algorithm. These numerical quantities will be clustered using the K-means algorithm. Lastly, the results will be presented using seaborn's plotting prowess and by displaying top keywords within each cluster.

# Improvements
### Webscraping:
1. Having more data (demographic data, dates, ratings, ect.) would allows for more interesting data exploration insights and more diverse features to improve cluster seperations. 
2. Additionally if this model would be applied to a large business with a steady stream of customer reviews, automatization and model refitting would be crucial towards gaining accurate insights at an acceptable speed. 
3. Lastly, there was significant cluster overlap because most of the reviews were positive. This model would be best suited for reviews with more diverse sentiments and opinions.

### Preprocessing
1. People tend to stack a lot of information about a different aspects of a business in a review. It is hard to cluster a multifaceted review since it is similar to many other documents due to its diverse nature. To combat this, a potential solutiion would be to seperate the review by sentences and cluster the sentences instead.
2. Once there is more data, I would implement lemmatization in the preprocessing step to reduce redundencies. 
3. The model had a slow drop-off in SSE as the number of clusters increased. Different algorithms should be texted (e.g. ELMo BERT) to see if better results and seperation can be achieved.

### Clustering
1. More data would improve clustering seperation. 
2. Again, more diverse data would improve cluster seperation. 

### Top Keywords
1. I would include a bargraph that compares the number of uses of the top words in each cluster. However, this would only work if there is a smaller number of clusters
2. Furthermore, displaying the review closest to the cluster center would offer more insight into the general opinion of the cluster
