# Nestlé Data Challenge

Which city Nestlé should expand "Vem de Bolo" platform through Moça program?

<img src="https://github.com/kaotcs/p005-allinoneplace/blob/main/img/785054-ecommerce-istock-020119.jpg" alt="All in one place"
	title="AIOP"  width="100%" height="500" />

## 01 BUSINESS PROBLEM
Assist the development of artisanal market with produces independently cakes and sweet
In which brazilian cities Moça should start a incentive program of gastronomic artisanal entrepreneurship
The proposal must consider the sustainability and scalability of the business.

## 02 BUSINESS ASSUMPTIONS
<ul>
<li>It was analyzed only data related to the cities (cognatis.csv)</li>
<li>"Vem de Bolo" data will be analyzed in the next cicle of CRISP </li>
</ul>

## 03 SOLUTION STRATEGY
The strategy adopted was the following:

<b>Step 01.</b> Data Description: Searching for missing values, checking data types and preliminary statistical description.

<b>Step 02.</b> Feature Engineering: Creating new features to improve the features for clustering.

<b>Step 03.</b> Data Filtering: Data with no information or containing inputs which does not match to the scope of the project were removed.

<b>Step 04.</b> Exploratory Data Analysis: Analyzed the features created by verifiy if is possible to make a cleaner dataframe for clustering. New features were created and other removed or improved.

<b>Step 05.</b> Data Preparation: Transforming the data for inputing to machine learning model. Most of jobs were rescaling and transforming the features values.

<b>Step 06.</b> Feature selection: Not Applied.

<b>Step 07.</b> Machine learning modelling: Identifying the best k for the cluster. It was used k-Means, GMM and Hierarchical Clustering and the metric employed to choose the best k was silhouette score.

<b>Step 08.</b> Hyperparameter Fine Tunning: It was employed K-means with k=4, since the embedded space did not have a overlap between clusters.

<b>Step 09.</b> Cluster Analysis: With 4 clusters created, it was chosen with the best average worker income.

<b>Step 10.</b> Exploratory Data Analysis for "Vem de Bolo" candidate: It was made a visual map to visualize the main insights

## 04 TOP 3 DATA INSIGHTS

* 82% of database is represeted by new customers or just made one order since the registration.

* Most of customers are from UK and Europe (up to 90%), but there are other from other countries.

* 117 customers indicated in the insiders cluster represent 7% of annual revenue.

## 05 MACHINE LEARNING MODEL APPLIED

The following machine learning algorithms were used to predict sales:

* k-Means;
* Gaussian Mixture Models (GMM);
* Hierarchical Clustering;

## 06 MACHINE LEARNING MODEL PERFORMANCE

The silhouette score for each model is indicated bellow:

<img src="https://github.com/kaotcs/p005-allinoneplace/blob/main/img/silhouette.jpg" alt="ML peformance"
	title="AIOP"/>

## 07 DEPLOYMENT
It was used AWS plataform (S3, RDS and EC2) to deploy the result of this clustering. The insiders clusters data can be visualized at Metabase platform. (Link will be available soon)

## 08 CONCLUSION
This insiders clusters represet a great path to marketing team and strategical aprouch to BI team improvement of revenue and keep the sales higher. The other customers which is not included should be analyzed and it is importante to create some trigger to pull them to insiders clusters.

## 08 LESSONS LEARNED / NEXT STEPS AND IMPROVEMENTS
Clustering problems is an unsupervised problem which does not have the right answer. It was made 9 cicles where it was made a deeper look in each feature. At this point, it was selected the best result that should be improved exploring new features or creating new ones from existing data.
