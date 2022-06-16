# Case title: Improving reverse logistics at PostNL

## Case background

Consumers in the Netherlands have the dubious honor to be the ones that send most online purchases back. In the Netherlands, there’s a return rate of 13 percent, which is more than in countries such as Germany, Poland and Switzerland. Reverse logistics handles these returns. Typically, a customer places an order for a return shipment in the webshop after which the returned goods are dropped at one of the many collections points. In the case of PostNL, there are xxxx of these collection points, located in supermarkets and convenience stores.



Orders for returns at webshops are placed until late in the evening. The capacity, sorting and route plans for the next few days have already largely been made by then. Hundreds of thousand containers are daily planned for the shipment of packaged goods. Data shows that on average at least 30% of the transport capacity is not utilized. Shortages or a surplus of available containers on a customer location, lead to inefficient logistics like delays, increasing CO2 emissions and additional costs.

Improving the expectation of the volume of packaged and containerised goods translates into an optimized supply chain planning. 
Online and physical stores have different characteristics. Some have highly seasonal volumes, others are very stable. We can use such information to more accurately predict the shipment of containerised goods released for transport.







For the logistic operations of containers, a Proof of Concept (PoC) is developed to optimize in real-time available container stock at customers (stores). One of the many pieces of the puzzle for a digital twin in logistics. During this PoC phase, the prediction model is deployed manually per customer. In the next phase the predictions are made by a request from a Control Tower application. A place where the expected volume of packaged and containerised goods is closely monitored and compared with the transport planning. 
Key for success is breaking down the bigger picture into multiple models per customer category that can be validated individually. This approach avoids major investments that later turn out to be unnecessary.

With the help of machine learning, decisions are no longer made based on assumptions but on data, which can be used to determine whether the expectation of the volume of packaged and containerised goods represents reality. As soon as a deviation occurs somewhere, the impact can be calculated to support decisions that are required to fulfill the customer promise.



## The challenge 

Sales of printed magazines have shrunk considerably since the advent of online media. Digitalisation creates many new opportunities for publishers, but obviously results in declining revenues from printed magazines year on year. Furthermore, shelf space in a supermarket is very expensive. These trends have challenged Aldipress and supermarket managers how to make a profit in a declining market. In essence, this boils down optimal matching of supply and demand of the many magazines across many different types of shops.

Traditionally, Aldipress' strategy was to sell as many magazines as possible, from as many publishers as possible, from as many points of sale as possible. Following a new business strategy in 2020, the approach for distribution of print magazines was changed to focus on a core assortment per store type. You can imagine this was a considerablt mind shift for a company which has been very successful with a “steady” business concept for decades.

## The results

To support this this new strategy with data analysis, Harm Bodewes stepped in and applied unsupervised machine learning to identify different different store types in a jungle of numerical data. Specifically, he used K-Means clustering which takes several numerical attributes as input to identify a pre-defined number (K) clusters. The outcome of the various runs of the clustering algorithm were analysed qualitatively to arrive at a practical set of store type. In addition, a core assortment and a uniform shelf layout was defined for each different store type. The solution was developed in April-September 2021 and is currently being implemented at SUPERUNIE and other supermarkets in The Netherlands.

![image](islr-figure-12.8.png)

Source: [Introduction to Statistical Learning, 2nd edition](https://www.statlearning.com/). Chapter 12: Unsupervised Learning.

The figure illustrates how these clusters are determined. The algorithm runs in several iterations, and every iteration has several steps. The objective of the algorithm is to assign a colour to each observation. In this example we see three different colours, so k=3. The example above is in the 2-dimensional space, you can see an x- and a y-axis. The power of the algorithm is that you can also run it in the n-dimensional space, which is obviously more difficult to visualize. In the Aldipress case we used a 40-dimensional space. 

We implemented this algorithm in a Python notebook. The input data came from both SAS (the forecasting “engine” of Aldipress) and SAP (the ERP system which contains all master data of Aldipress). Below you find the output for SUPERUNIE stores with 3 metres shelf space.

Based on the output, Aldipress defined 3 store types: BUDGET, FAMILY and PREMIUM. In BUDGET stores, Aldipress will place more TV Guides (who is still buying TV magazines in 2022 by the way?) and Gossip. In PREMIUM Aldipress will supply more Glossies and Woman-magazines. The category FAMILY is “for everybody something”.

The cluster analysis contains very relevant information for Aldipress, as this solution can minimise return cost and the risk of out-of-stock by making a good estimation of number of magazines to be sold. The supermarket manager is also happy with this solution, as he/she will only sell magazines which the consumer really wants. The small publishers with very specific magazines might be less happy and will look for other ways of distribution.

## Testimonial

<How did the alumnus/alumni apply her/his experience at JADS in this case? How would she/he describe this to others?>

## Facts

- Company: Aldipress
- Lead Data Scientist: Harm Bodewes
- Type of collaboration: in-company project JADS Professional Education 
