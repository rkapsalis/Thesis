# ⚖ Research and development of a system for bias identification in recommender systems
![image](https://user-images.githubusercontent.com/48930309/198666695-e314fec9-f35b-4c28-b218-5940e2d77e60.png)
## 📕 Abstract
<div align= "justify">
Recently, researchers have increased their scrutiny of ethical issues on artificial intelligence (AI), especially οn the field of Machine Learning. However, most previous studies on the area of Ethical Machine Learning have only focused on classification and regression tasks,  while only a few studies have investigated ethical issues on recommender systems.
The aim of this Diploma Thesis is to contribute to the understanding of biases that appear in recommender systems. 

In this direction, a web-app was developed to help users understand how biases are introduced in recommender systems. Moreover, we could thereby estimate the extend of bias in these systems. The app is comprised by four main pages. The first page visualizes datasets to help users find possible biases. In the second page, the user can build a recommender system by choosing between a vast collection of algorithms and hyperparameter tuning options in a user-friendly way. Additionally, we developed a page for the evaluation of a recommender system as per popularity bias, fairness, diversity, novelty and coverage. The evaluation consists of a) bias monitoring through different types of plots for a single dataset or dataset comparison b) cut-off analysis and c) hyperparameter analysis. Finally, we developed a page for popularity bias mitigation using one of the four algorithms that are available:  FAR, PFAR, FA*IR and Calibrated recommendations.

With reference to the broader field of ethical issues, this thesis shares special interest to popularity bias, diversity, novelty and item coverage. An extensive experimental study was conducted to gain a better understanding of the sources of bias and analyze the effect of different bias mitigation algorith\-ms. This was implemented by utilizing the aforementioned web app. Four datasets were used in the present study: one real dataset provided by a major electronics retailer, and three datasets collected from the internet.
The first part of the study examines the role of the hyperparameter tuning for every algorithm that was used and the role of dataset characteristics, in bias and accuracy. It also compares the above-mentioned datasets. The second part consists of bias mitigation using three re-ranking algorithms: FAR, PFAR and Calibrated recommendations and an in-processing algorithm.

This study has identified that data characteristics, and especially the sparsity of user-item matrix, can highly affect the bias that is introduced. Moreover, another significant finding is that the post-processing mitigation algorithms that were examined can improve the bias-accuracy tradeoff, but have several limitations too.
In conclusion, developers of recommender systems need to be aware of sources of biases and of the accuracy-bias tradeoff. This work contributes to this direction and
lays the groundwork for future research into bias in recommender systems.
</div>

## 💻 Streamlit app
### Visualize data
| ![image](https://user-images.githubusercontent.com/48930309/198675351-a43220a1-cd58-4097-aebb-751e41ffd920.png) |
|:--:|
| <b>Useful information about Movielens1M dataset</b>|

In this page, the user can get a qualitative understanding of the data via getting useful information and statistical details for the dataset and via 4 main types of plots that are offered:

<details><summary>Most rated itemss</summary>
<p>
 
![image](https://user-images.githubusercontent.com/48930309/198682956-3186bc8b-f1b2-4586-ac03-762430585110.png)
 
</p>
</details>

<details><summary>Top users</summary>
<p>
 
![image](https://user-images.githubusercontent.com/48930309/198683638-2fc84135-fb07-42d9-9184-3b33d98eb1ea.png)
 
</p>
</details>

<details><summary>Long tail</summary>
<p>
 
![image](https://user-images.githubusercontent.com/48930309/198683765-feb7e3d2-94da-4cbf-a231-9510ba518ae3.png)
 
</p>
</details>

<details><summary>Average number of ratings</summary> 
<p>
 
![image](https://user-images.githubusercontent.com/48930309/198683718-f46bcaee-fcc6-4a99-a88e-9a2d22b00a7b.png)
 
</p>
</details>



### Build recommendation system
The user can also build a recommendation system, choosing from a variety of algorithms and evaluation metrics, provided by [Elliot framework](https://github.com/sisinflab/elliot). 
![image](https://user-images.githubusercontent.com/48930309/198673033-b0e23409-9b63-43a1-9b3e-79cadc8c7093.png)
![image](https://user-images.githubusercontent.com/48930309/198673266-bc6a128f-892d-4540-9c45-a514e6c85b4b.png)



He can use the default values of the hyperparameters of every algorithm or set his preferred values (for more experienced users):

![image](https://user-images.githubusercontent.com/48930309/198674292-39bde047-4913-4ea7-a202-dcd2345c957d.png)

### Bias identification
After building a recommender system, the user can analyze the generated recommendations by using the evaluation metrics of his preference. There are 24 metrics available including accuracy, popularity bias, coverage, diversity and novelty metrics, provided by Elliot framework. You can either analyze the results of a single dataset or compare the results of different datasets. 
<details><summary>Best results</summary>
<p>

#### Best results
![image](https://user-images.githubusercontent.com/48930309/198676083-4e5e7333-9cea-4700-b94e-54b912be476d.png)



</p>
</details>

<details><summary>Hyperaparameter analysis</summary>
<p>


![image](https://user-images.githubusercontent.com/48930309/198676778-99d260ba-6b8e-41d4-b40c-01bc77d6622a.png)

</p>
</details>

<details><summary>Cutoff analysis</summary>
<p>

![image](https://user-images.githubusercontent.com/48930309/198676163-70a5fa7f-ad2d-4b46-840b-fad41a4888b9.png)

</p>
</details>
<details><summary>Dataset comparison</summary>
<p>

![image](https://user-images.githubusercontent.com/48930309/198677162-8f2f15d9-8a9e-467f-9067-f8a1d674fa9d.png)

</p>
</details>

### Bias mitigation
The bias mitigation technique used, belongs to the category of post-processing techniques, and more specifically to the re-ranking algorithms. These techniques take as input a recommendation list for every user in the dataset, produced by an algorithm of your choice. There are 3 bias mitigation algorithms, available in our app: FAR, PFAR and FA*IR. These algorithms are provided by [Librec-auto](https://github.com/that-recsys-lab/librec-auto).
 
![image](https://user-images.githubusercontent.com/48930309/198679870-33f89129-6320-4121-89e9-7536e76df0bb.png)

When the bias mitigation process has been completed, plots comparing the results produced by the technique with the initial results are shown. 

### Metrics explanation
The app provides also detailed and simple explanations in non-technical terms, for all the evaluation metrics contained in our app:
![image](https://user-images.githubusercontent.com/48930309/198674718-ab38570d-480f-4007-94bd-88e803a17d0c.png)
![image](https://user-images.githubusercontent.com/48930309/198674819-f959c827-fc03-40d3-9333-938524ec6daa.png)

### Upload data
![image](https://user-images.githubusercontent.com/48930309/198674899-5509ad2f-17b5-486b-8615-9dd635a2947f.png)

## 📜 License
[Creative Commons Zero v1.0 Universal](https://github.com/rkapsalis/Thesis/blob/main/license.md)
