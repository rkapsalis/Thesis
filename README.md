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
![image](https://user-images.githubusercontent.com/48930309/198675351-a43220a1-cd58-4097-aebb-751e41ffd920.png)

- Most rated items
- Top users
- Average number of ratings
- Long tail
### Build recommendation system
![image](https://user-images.githubusercontent.com/48930309/198673033-b0e23409-9b63-43a1-9b3e-79cadc8c7093.png)
![image](https://user-images.githubusercontent.com/48930309/198673266-bc6a128f-892d-4540-9c45-a514e6c85b4b.png)
![image](https://user-images.githubusercontent.com/48930309/198674292-39bde047-4913-4ea7-a202-dcd2345c957d.png)

### Bias identification
- Hyperaparameter analysis
![image](https://user-images.githubusercontent.com/48930309/198676778-99d260ba-6b8e-41d4-b40c-01bc77d6622a.png)
- Best results
![image](https://user-images.githubusercontent.com/48930309/198676083-4e5e7333-9cea-4700-b94e-54b912be476d.png)

- Cutoff analysis
![image](https://user-images.githubusercontent.com/48930309/198676163-70a5fa7f-ad2d-4b46-840b-fad41a4888b9.png)

- Dataset comparison
![image](https://user-images.githubusercontent.com/48930309/198677162-8f2f15d9-8a9e-467f-9067-f8a1d674fa9d.png)

### Bias mitigation
### Metrics explanation
![image](https://user-images.githubusercontent.com/48930309/198674718-ab38570d-480f-4007-94bd-88e803a17d0c.png)
![image](https://user-images.githubusercontent.com/48930309/198674819-f959c827-fc03-40d3-9333-938524ec6daa.png)

### Upload data
![image](https://user-images.githubusercontent.com/48930309/198674899-5509ad2f-17b5-486b-8615-9dd635a2947f.png)


