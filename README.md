# Netflix Movies and TV Shows Clustering Project

## Introduction

Welcome to the Netflix Movies and TV Shows Clustering Project! In this project, we delve into a dataset containing a variety of movies and TV shows available on the Netflix platform. Our primary goal is to perform text-based clustering to group similar content together in clusters.

## Exploratory Data Analysis (EDA)

During our exploratory analysis, we uncovered fascinating insights:

- There's a notable abundance of movies compared to TV shows on Netflix.
- Over the past 15 years, the quantity of content on Netflix has surged dramatically, with a specific focus on TV shows.
- The United States leads with the highest volume of content, while India boasts the highest number of movies.
- The majority of the content caters to an audience aged 18 and above.

## Feature Engineering

To facilitate our clustering analysis, we selected the following text-based features for both movies and TV shows:

- Cast
- Country
- Rating
- Listed_in (genre)
- Description

To preprocess the textual data, we executed tasks such as punctuation and stopword removal. Employing the TF-IDF vectorizer, we transformed the textual content into a numerical format, generating a feature matrix with 5000 dimensions.

## Dimensionality Reduction

Acknowledging the presence of numerous features, we harnessed Principal Component Analysis (PCA) for dimensionality reduction. After rigorous experimentation, we found that retaining 80% of the variance with 3000 features led to optimal outcomes.

## Clustering Models

We embarked on an exploration of two prominent clustering algorithms: K-Means clustering and Hierarchical clustering.

### K-Means Clustering

To pinpoint the ideal number of clusters for K-Means, we harnessed the power of the Elbow Method and Silhouette Analysis. Through careful analysis, we concluded that creating '7' clusters would be most effective. While K-Means proved adept at grouping similar content, some clusters exhibited less distinct characteristics.

### Hierarchical Clustering

In the realm of Hierarchical clustering, we harnessed the capabilities of a dendrogram to determine the optimal cluster count. Our analysis pointed us toward creating '8' clusters. Leveraging Agglomerative Clustering for grouping, this approach yielded more well-defined clusters compared to K-Means.

## Conclusion

In summation, our project triumphantly organized Netflix movies and TV shows into clusters based on textual attributes. Our findings show that Hierarchical Clustering delivered clusters with more pronounced distinctions compared to K-Means. This analysis holds potential for enhancing recommendation systems, content structuring, and deepening our understanding of user preferences on the Netflix platform.

Feel free to explore the code and insights shared in this repository. We hope this project sheds light on the power of clustering and its real-world applications in content categorization and analysis.

Thank you for visiting our Netflix Movies and TV Shows Clustering Project!
