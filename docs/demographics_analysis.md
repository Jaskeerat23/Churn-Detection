# **Demographics Analysis** 

The main demographical features the dataset had were :
1. Customer_Age
2. Gender
3. Dependent_Count
4. Marital_Status
5. Education_Level
6. Income_Category
7. Card_Category

## Customer_Age :

`Customer_Age` have been visualized using 2 **historgram plots**, one for displaying **total customers in each bin** and another for **customers churned in each bin**. The Bins are constructed from the minimum age divisible by 5 to maximum age with step of 5. E.g. `[5, 10, 15, 20]`.

The plots are:

<p allign="center">
  <img src="D:/Churn Detection/Plots/customer_age-1.png" alt="Centered image">
</p>
<p allign="center">
  <img src="D:/Churn Detection/Plots/customer_age-2.png" alt="Centered image">
</p>

From the First Plot we can see that the customer age distribution is following a *normal distribution*. And the majority of the customer belong to the **age group of 45-50**. From the second plot also we can see that the customers that fall in this age group **churns a lot and their churn rate is pretty high** as comapred to any other group. So they fall under risk zone.

### Note :
For some categorical variables instead of plotting them we made a table for them to analyze them

## Gender:

The analysis of this feature is available in the file `EDA\Gender_categorical_analysis.csv`. 
Gender is not a strong predictor for churn as their is no gurantee whether someone will churn or not based on their gender, as a woman earning good may also churn where as a man not earning good may not churn.
So this feature must not be given a significant weight in modeling.

## Marital Status :

The analysis of this feature is availabel in the file `EDA\Marital_Status_categorical_analysis.csv`. This feature is not very strong for feature modeling. The reason behind it depends on the income category of the person who got divorced or earning etc.

## Education Level :

This is one of the **best** demographical feature that we can use in our Model. The reason behind it is very clear, if we look at the csv we can see that the customers who are just **high school grads have a very low churn rate i.e. they are very unlikely to churn** since they don't have that much education to support there family or live a good lifestyle where as the **customers who are doctrates chrun alot** since they have a qualification which is generally paid well in today's time.

The churn rate varies from *15.2% ~ 21.06%* with high school grads being the lowest and doctrates being the highest.

So this is a very good feature that we can use in our model as well as for knowledge base.

## Income Cateogry :

Again a very strong feature like `Education Level`, the reason is if we look carefully there are 2 known categories that churn a lot that is customers with **income less than $40K and customers above $120K**. The hypothesis can be that the person earning less than $40K have convinced itself to not use credit a lot since there income is not enough where as person earning above $120K already have a good income so they don't have any need to use credit card for small or medium size purchases.

So this feature must be kept during modeling since it is a strong signal and also used with other features can tell a lot about whether the person will churn or not.

## Dependent_Count :

<p allign="center">
  <img src="D:/Churn Detection/Plots/customer_age-2.png" alt="Centered image">
</p>

From the plot it is very clear that this plot does not convey a very strong signal about churn, however using this feature with some other feature like income category can convey something meaningfull. But alone this is a weak signal.