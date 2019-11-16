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
+ Project summary: Matrix factorization is a common machine learning technique for recommender systems, like books for Amazon or movies for Netflix. 
![](https://github.com/TZstatsADS/fall2019-project4-sec2-grp10/blob/master/figs/img1.png)
The idea of these methods is to approximate the user-movie rating matrix R as a product of two low-rank matrices U and V such that R ≈ U × V . In this way U and V are constructed from the known ratings in R, which is usually very sparsely filled. The recommendations can be made from the approximation U × V which is dense. If M × N is the dimension of R then U and V will have dimensions M × K and N × K. Noise is added to the model to avoid overfitting.
	
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
