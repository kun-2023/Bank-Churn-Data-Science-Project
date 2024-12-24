<h1>Bank-Churn-Data-Science-Project</h1>
<h2>Table of Content</h2>
<ul>
  <li>Dashboard Preview</li>
  <li>Background and Overview</li>
  <li>Executive Summary</li>
  <li>Insights and Deep Dive</li>
  <li>Machine Learning Model and Walk Through</li>
  <li>Reccomandations</li>
</ul>
<h3>DashBoard Preview</h3>

![European Banks Dashboard](https://github.com/user-attachments/assets/61944cf6-c3b5-4a89-ab32-87495fea2252)

<p>An interactive tableau dashboard could be accessed <a href="https://public.tableau.com/app/profile/kun.bi/viz/european_bank/EuropeanBankChurnDashboard">here</a>.</p>



<h3>Background and Overview</h3>
<p>This European bank is currently operating in France, Spain and Germany and provides services such as deposits management, credit card services and membership benefits. According to the latest datasets regarding to its 10000 customers of the bank, roughly 20% of the customers had chosen to close their bank account for good. That was a big loss for the bank. To help bank reduce churn rate, I decided to apply an EDA to discover the hidden patterns behind the churns and a Kneighborclassfication machine learning model to help predict the churn or unchurn outcomes.</p>
<h3>Data Structures</h3>

![data_structures](https://github.com/user-attachments/assets/295a9ae3-3567-4055-a361-ece60a53b40a)

<h3>Executive Summary</h3>
<ol>
  <li>Germany has the lowest customers but the highest churn rate. France has the most customers but the lowest churn rate. Spain has a similar churn rate as France with only 50% of France’s customers.</li>
  <li>Male customers are 20% more than the female customers, but the female churn rate is higher than male at 25% vs 16%.</li>
  <li>Customers with 2 products have a low churn rate at 7.6% and it also has the highest number of customers. Customers with above 2 products have above 80% churn rate. </li>
  <li>Active member has much lower churn rate than non active member at 14.26% vs 27%.</li>
  <li>For people at age between 40 and 65 have a churn rate of 39%, which is almost 4 times as high as clients from other demographics, which was standing at 10.8%. However, for clients below age of 40, it totaled at a population of 6419 with a churn rate of 10.87%. </li>
</ol>

<h3>Insights Deep Dive</h3>
<p>The features are related the most to the churns are Geography, Gender, Number of Products, Membership.</p>
<p>The Datasets is Bank Customer Churn from <a href="https://mavenanalytics.io/data-playground?order=date_added%2Cdesc&search=bank">Maven Analytics Data Playground</a>. The EDA and machine learning model were written in python libraries such as pandas, seaborn, matplotlib, and sklearn. To see the technical details, olease take a look at the uploaded notebooks.</p>
<h4>Geography and churn</h4>
<p>
  France has the most amount of customers of 5014 compairing to Germany of 2509, Spain od 2064. However, the churn rate in Germany is the highest at 32.44% which is twice as high as the churn rate in Spain or France. The churns in Germany is also much more concentrated for people between age of 40 and 60 while in France and Spain, it much less intense.
</p>

![country_churn](https://github.com/user-attachments/assets/83a379e6-590c-471c-aaec-ce53ca9c876b)



![country_nation_churn](https://github.com/user-attachments/assets/60d53525-2178-4587-b746-24a0c4f3e0e9)

<h4>Gender and Churn</h4>
<p>There are more male customers than female customers, but there are more churns in terms of both churn number and churn rate in female than male.</p>

![gender and churn](https://github.com/user-attachments/assets/976fa37e-fbeb-449e-895a-501f40e1a5ab)

<h4>NUmber of products and churns</h4>
<p>Clients with 3 and 4 products had almost closed their accounts. However, clients with one products have a high but much more normal churn rate of 27%. Clients having two products have a low churn rate of 7.5%</p>

![numofproducts and churn](https://github.com/user-attachments/assets/eb4500b1-934d-4803-b1fc-e6cb6e63c81e)

<h4>Membership and Churn</h4>
Clients in a membership have a much lower churn rate of 14.27% compairing to the clients not in a membership of a churn rate of 26.86%. Membership help clients stay with the banks longer. For clients not in a membership, most of churns took place between 45 and 70.

![membershio and churn](https://github.com/user-attachments/assets/5dae92e3-e619-4e13-8027-748c1d034d99)

![age_membership_churn](https://github.com/user-attachments/assets/ebfd0439-19e5-4c2b-8b7a-14eb34bb618d)



<h4>Age and churn</h4>
<p>Age has a striking relationship with churns. It turns out that clients between age of 40 and 65 have a churn rate of 39% in contrast to clients, otherwise, with a churn rate of 10%. People at age of 40 and 65 are very likely to close their bank accounts. Clients with credit scores of 400 or less  had totally closed their accounts. </p>


![age and churn](https://github.com/user-attachments/assets/ef009f61-1c98-43b4-8e96-51bb88e3562f)




![age_segment_churn](https://github.com/user-attachments/assets/fbd18790-1bb6-4ba4-8f82-625e3484e610)

<h3>Machine Learning Model Walk Through</h3>
<p>I choose K Nearest Neighbors classification models to train the datasets to build the predictive model. I picked 11 as the optimized number of neighbors for classification.</p>

![knn_optimized_k](https://github.com/user-attachments/assets/e8097fd4-57c0-45a3-a7d1-d53139075fff)

<p>Here are the evaluation of the model. The train score is 85%, and the test score is 84%. The model has a high accuracy not overfit. However, it does have a precision score of 71% and a low recall score of 37% for the positive case.</p>

![knn_evaluation](https://github.com/user-attachments/assets/988b58bb-ba93-4dab-8b16-c2ad207268c0)
<p>The precision-recall curves are show the precision score and recall score are at each other's expenses. It's not possible to have a point where the model can enjoy a high precision and a high recall score at the same time.</p>


![precision-recall-curve](https://github.com/user-attachments/assets/5fa37c78-d997-42dc-a0f4-320a97e72fa1)

<p>The model has a roc curve with an AUC of 89%. It means the model have an accuracy of 89% of correctly classifying a given case all in all.</p>

![roc_curve](https://github.com/user-attachments/assets/6fd729e4-9f84-4b55-a9d5-a65664f3e83c)


<h3>Recommandations</h3>
<ol>
  <li>Reduce business in Germany while try to expand in France and especially Spain. Spain has similar churn rate as France, both clients number and churn rate of which are significantly lower than Germany’s.</li>
  <li>Convert customers with one product to have 2 products before they shut down the accounts. Prevent customers from having more than 2 products, it could end up too financially draining for them to keep their accounts.</li>
  <li>Provide more engagement to non member customers so they would become active member and use the account more often. </li>
  <li>Engage new customers at age between 18 and 45 to preserve a low churn rate as possible.</li>
  <li>Avoid clients with a credit score of less than 400 or help clients' crdit scores stay above 400. </li>
</ol>


