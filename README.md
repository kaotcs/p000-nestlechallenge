# Nestlé Data Challenge

Which city Nestlé should expand "Vem de Bolo" platform through Moça program?

<img src="https://github.com/kaotcs/p000-nestlechallenge/blob/main/img/cover.png" alt="Cover"
	title="cover"  width="100%" height="500" />

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

## 04 TOP 4 DATA INSIGHTS FROM "VEM DE BOLO" CANDIDATE CLUSTER

<img src="https://github.com/kaotcs/p000-nestlechallenge/blob/main/img/cluster01.png" alt="cluster01"
	title="Nestle"/>

* 100% of greatest cities in Brazil are included in this cluster and 98% have their population still expanding.

* 31% of total have average income above R$ 4.400 (middle class).

* 90% of the municipalities have at least 5.000 workers around of area where the analyzes were made. (great capacity of earning)

* 100% of the municipalities concentrate small businesses (entrepreneur) around of area where the analyzes were made.

## 05 MACHINE LEARNING MODEL APPLIED

The following machine learning algorithms were used to predict sales:

* k-Means;
* Gaussian Mixture Models (GMM);
* Hierarchical Clustering;

## 06 MACHINE LEARNING MODEL PERFORMANCE

The silhouette score for each model is indicated bellow:

<img src="https://github.com/kaotcs/p000-nestlechallenge/blob/main/img/score_silhouette.jpg" alt="ML peformance"
	title="Nestle"/>

## 07 CONCLUSION
This work was developed to Nestlé Data Challenge where it was possible to point which cities them should look for the expansion of "Vem de Bolo" platform. It was possible to see 381 cities where they could make further investigation, but we can indicate a TOP 10 cities where they can start:

<img src="https://github.com/kaotcs/p000-nestlechallenge/blob/main/img/top10.png" alt="top10"
	title="Nestle"/>

Complete ranking: https://docs.google.com/spreadsheets/d/1bq9jd3d8fwLpyxI6qVphuSv8LDtpNLsH/edit#gid=450600250

This project was presented to Nestlé in December 10th, 2021 and won the 4th place in this Data Challenge.

## 08 LESSONS LEARNED / NEXT STEPS AND IMPROVEMENTS
Since it was given only one week to analyzed the data, it was not possible to develop others database provided by "Vem de Bolo". In next cicles, it should be made a deeper investigation to acomplish all IOT checklist indicated at the beginning of the project.
