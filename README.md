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

![Images](data:image/png;base64,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)

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
