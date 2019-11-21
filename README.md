# Project 4: Algorithm implementation and evaluation: Collaborative Filtering

### [Project Description](doc/project4_desc.md)

Term: Fall 2019

+ Team 10
+ Projec title: Recommender System using SGD and GDP based on KNN
+ Team members
	+ Weijia Bao
	+ Tiantian Chu
	+ Qiwen Gao
	+ Yanyan Liu
	+ Mo Yang
+ Project summary: Recommender systems are crucial to e-commerce. If companies, like books for Amazon or movies for Netflix, can target customers with personalized products, they can build up customers’ loyalty and satisfaction.

+ We tuned the parameters and then we compared the RMSEs to find our best model for each algorithm. We Compared the results of the plots. We found the lowest RMSE of testing data is f=10, and lambda =0.1. we found the pattern of the points follow the gradually descended.

Stochastic Gradient Descent 

![](https://github.com/TZstatsADS/fall2019-project4-sec2-grp10/blob/master/figs/Stochastic Gradient Descent.png)

Gradient Descent with Probabilistic Assumptions

![](https://github.com/TZstatsADS/fall2019-project4-sec2-grp10/blob/master/figs/Gradient Descent with Probabilistic Assumptions.png)

+ Then we use KNN. K=1 to find the nearest movie for each movie, and calculate the mean score of k features. After that, we built linear regression to optimize the rating accuracy and calculated the final prediction of the rating. 

+ Last, we got the conclusion, it will take more time, even though the RMSE will get better, and result of this two models are similar, after the postprocessing with KNN, model does not have a significant impact on the accuracy.


In this project, we applied the following proposed methods to IMDB movie datasets:
SGD(Stochastic Gradient Descent)
GDP(Gradient Descent with Probabilistic Assumptions)

![](https://github.com/TZstatsADS/fall2019-project4-sec2-grp10/blob/master/figs/img1.png)

The idea of these methods is to approximate the user-movie rating matrix R as a product of two low-rank matrices U and V such that R ≈ U × V. In this way U and V are constructed from the known ratings in R, which is usually very sparsely filled. The recommendations can be made from the approximation U × V which is dense. If M × N is the dimension of R then U and V will have dimensions M × F and N × F.

p.s. To implement GDP, we need to firstly do probabilistic matrix factorization. The Gradient Descent algorithm consists of updates in the direction that minimizes L(U, V) until convergence.
 
 
with partial differential
 

**Contribution statement**: [default] All team members contributed equally in all stages of this project. All team members approve our work presented in this GitHub repository including this contributions statement. 

Following [suggestions](http://nicercode.github.io/blog/2013-04-05-projects/) by [RICH FITZJOHN](http://nicercode.github.io/about/#Team) (@richfitz). This folder is orgarnized as follows.

```
proj/
├── lib/
├── data/
├── doc/
├── figs/
└── output/
```

Please see each subfolder for a README file.
