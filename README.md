<h1>Bank-Churn-Data-Science-Project</h1>
<h3>Description</h3>
<p> This project is regarding to a datasets of the customer churn of an European bank operating in Spain, Germany, and France. Recently, this European bank has been losing customers. To improve the bank's performence, I would be conducting an EDA to discover the pattern and the features mosted related to the churn rate and establish a machine learning model to predict the churn given a customer's features.  </p>
<h3>Executive Summary</h3>
<ol>
  <li>Germany has the lowest customers but the highest churn rate. France has the most customers but the lowest churn rate. Spain has a similar churn rate as France with only 50% of France’s customers.</li>
  <li>Male customers are 20% more than the female customers, but the female churn rate is higher than male at 25% vs 16%.</li>
  <li>Customers with 2 products have a low churn rate at 7.6% and it also has the highest number of customers. Customers with above 2 products have above 80% churn rate. </li>
  <li>Active member has much lower churn rate than non active member at 14.26% vs 27%.</li>
  <li>For people at age between 40 and 65 have a churn rate of 39%, which is almost 4 times as high as clients from other demographics, which was standing at 10.8%. However, for clients below age of 40, it totaled at a population of 6419 with a churn rate of 10.87%. </li>
  <li>Clients with balance less than 10000 euros had all churned.</li>
</ol>
<h3>Recommandations</h3>
<ol>
  <li>Reduce business in Germany while try to expand in France and especially Spain. Spain has similar churn rate as France, both of which are significantly lower than Germany’s.</li>
  <li>Try to convert customers with one product to have 2 products before they shut down the accounts. Prevent customers from having more than 2 products, it could end up too draining for them to keep the account.</li>
  <li>Provide more engagement to non member customers so they would become active member and use the account more often. </li>
  <li>Engage new customers at age between 18 and 40 to have a low churn rate as possible and also with a balance above 10000 Euros.</li>
</ol>
<h3>Analysis</h3>
<p>The Datasets is Bank Customer Churn from <a href="https://mavenanalytics.io/data-playground?order=date_added%2Cdesc&search=bank">Maven Analytics Data Playground</a>. The EDA and machine learning model were written under python libraries such as pandas, seaborn, matplotlib, and sklearn.</p>
<p>
  France has the most amount of customers of 5014 compairing to Germany of 2509, Spain od 2064. However, the churn rate in Germany is the highest.
</p>

![country_churn](https://github.com/user-attachments/assets/83a379e6-590c-471c-aaec-ce53ca9c876b)




