# Research and development of a system for bias identification in recommender systems
## Abstract
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
