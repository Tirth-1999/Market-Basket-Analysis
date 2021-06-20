# Market-Basket-Analysis
 > <b>Often wonder how you come to a mall with strict bubget but always end up breaking it, cause you thought it's a great deal ?</b>

 ![Market Basket](https://images.unsplash.com/photo-1578916171728-46686eac8d58?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=667&q=80)

```
> What Actually is Market Basket Analysis? 
```
 Market basket analysis is a __data mining__ technique used by retailers to increase sales by better understanding customer purchasing patterns. It involves analyzing large data sets, such as purchase history, to reveal product groupings, as well as products that are likely to be purchased together.

 ```
 > How does it actually work in real life?
 ```
 Market Basket Analysis is one of the key techniques used by large retailers to uncover associations between items. __<u>It works by looking for combinations of items that occur together frequently in transactions. To put it another way, it allows retailers to identify relationships between the items that people buy.</u>__

 In order to make it easier to understand, think of Market Basket Analysis in terms of shopping at a supermarket. Market Basket Analysis takes data at transaction level, which lists all items bought by a customer in a single purchase. The technique determines relationships of what products were purchased with which other product(s). 

 ```
 > So how to find such Association Rules?
 ```

 Association Rules are widely used to analyze retail basket or transaction data, and are intended to identify strong rules discovered in transaction data using measures of interestingness, based on the concept of strong rules.
 
 
 These relationships are then used to build profiles containing If-Then rules of the items purchased. for example:
 
 `
    If {A} Then {B} : A => B
 `

![Images](http://www.saedsayad.com/images/AR_1.png)

So to start we need to be introduced to few technical terms :

1. __Support__ : Support is an indication of how frequently the item set appears in the data set. Mathematically,

 ![Images](https://webfocusinfocenter.informationbuilders.com/wfappent/TLs/TL_rstat/source/images/rstat_SupportFormula.jpg)

2. __Confidence__ : The confidence of the rule is the ratio of the number of transactions that include all items in {B} as well as the number of transactions that include all items in {A} to the number of transactions that include all items in {A}. Mathematically,

![Images](https://webfocusinfocenter.informationbuilders.com/wfappent/TLs/TL_rstat/source/images/rstat_ConfidenceFormula.jpg)

3. __Lift__ :  The third measure called the lift or lift ratio is the ratio of confidence to expected confidence. Expected confidence is the confidence divided by the frequency of B. The Lift tells us how much better a rule is at predicting the result than just assuming the result in the first place. Greater lift values indicate stronger associations. Simply, The lift of a rule is the ratio of the observed support to that expected if X and Y were independent.
Mathematically,

![Images](https://webfocusinfocenter.informationbuilders.com/wfappent/TLs/TL_rstat/source/images/rstat_LiftFormula_new.jpg)

For Example :
- Assume there are 100 customers
- 10 of them bought milk, 8 bought butter and 6 bought both of them.
- bought milk => bought butter
- support = P(Milk & Butter) = 6/100 = 0.06
- confidence = support/P(Butter) = 0.06/0.08 = 0.75
- lift = confidence/P(Milk) = 0.75/0.10 = 7.5



```
> Practical Applications of Market Basket Analysis
```
When one hears Market Basket Analysis, one thinks of shopping carts and supermarket shoppers. It is important to realize that there are many other areas in which Market Basket Analysis can be applied. An example of Market Basket Analysis for a majority of Internet users is a list of potentially interesting products for Amazon. Amazon informs the customer that people who bought the item being purchased by them, also reviewed or bought another list of items. A list of applications of Market Basket Analysis in various industries is listed below:
1. __Retail__. In Retail, Market Basket Analysis can help determine what items are purchased together, purchased sequentially, and purchased by season. This can assist retailers to determine product placement and promotion optimization (for instance, combining product incentives). Does it make sense to sell soda and chips or soda and crackers?
2. __Telecommunications__. In Telecommunications, where high churn rates continue to be a growing concern, Market Basket Analysis can be used to determine what services are being utilized and what packages customers are purchasing. They can use that knowledge to direct marketing efforts at customers who are more likely to follow the same path.

3. __Banks__. In Financial (banking for instance), Market Basket Analysis can be used to analyze credit card purchases of customers to build profiles for fraud detection purposes and cross-selling opportunities.

4. __Insurance__. In Insurance, Market Basket Analysis can be used to build profiles to detect medical insurance claim fraud. By building profiles of claims, you are able to then use the profiles to determine if more than 1 claim belongs to a particular claimee within a specified period of time.

5. __Medical__. In Healthcare or Medical, Market Basket Analysis can be used for comorbid conditions and symptom analysis, with which a profile of illness can be better identified. It can also be used to reveal biologically relevant associations between different genes or between environmental effects and gene expression.

And many more fields to cover, but for now you have understood it well.

Hope this article find you something good. 
```python
if Good == "Yes":
    print("Please show your love through Claps 👏, Love 🤍 and sharing it to others 👩‍🤝‍🧑🏼")
else :
    print("Would surely improve more to get to your satisfaction!")
