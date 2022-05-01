# Case: Aldipress

- Company: Aldipress
- Lead Data Scientist: Harm Bodewes
- Type of collaboration: in-company project JADS Professional Education 

## Sell less - make more money

Aldipress has been the market leader in distribution and marketing of magazines, comics, novels and puzzles in the Netherlands for over 50 years. As a partner for publishers and retailers, Aldipress' core business is to find effective solutions for assortment management, circulation management, shelf presentations and promotions. It was acquired by DPG in 2019 and currently serves:

-	120 publishers
-	1.100 magazines
-	5.200 points of sale (supermarkets, bookstores, gas stations, hospitals)

![image](https://aldipress-site.storage.googleapis.com/wp-content/uploads/20220425095624/Logo_Aldipress_2323x1550-1-1.jpg)

__\[start purple block\]__
  
## The challenge 

Sales of printed magazines have shrunk considerably since the advent of online media. Digitalisation creates many new opportunities for publishers, but obviously results in declining revenues from printed magazines year on year. Furthermore, shelf space in a supermarket is very expensive.

These trends have challenged Aldipress and supermarket managers how to make a profit in a declining market. In essence, this boils down optimal matching of supply and demand of the many magazines across many different types of shops.

## The solution

Traditionally, Aldipress' strategy was to sell as many magazines as possible, from as many publishers as possible, from as many points of sale as possible. Following a new business strategy in 2020, the approach for distribution of print magazines was changed to focus on a core assortment per store type. You can imagine this was a considerablt mind shift for a company which has been very successful with a “steady” business concept for decades.

Of course, this new strategy should be supported by data analysis, and this is where Harm Bodewes stepped in.
The solution was:
-	using K-means Clustering to identify different store types in a jungle of numerical data.
-	performing a qualitive analysis on the outcomes of the clustering algorithm.
-	defining a core assortment and a uniform shelf layout for each different store type. 

The solution was developed in April-September 2021 and is currently being implemented at SUPERUNIE and other supermarkets in The Netherlands.

## Techniques applied

The K-Means clustering method has:
-	as input several different numerical attributes. 
-	as optional input a value of “k”, which is equivalent to the number of clusters you want.
-	as output k clusters, which are calculated according to the algorithm below.
![image](https://user-images.githubusercontent.com/4090894/166159227-50a6daf1-c6af-4fd0-b2a3-fd68fb0a5462.png)




