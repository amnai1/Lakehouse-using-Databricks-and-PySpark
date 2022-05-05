# Lakehouse using Databricks and PySpark

We will build a lakehouse architecture utilising delta lakes, an end to end ELT pipeline in Azure Databricks, along with some near-real-time dashboards. Since this is Databricks, the example is more programmer friendly as the entire pipeline is in python or more specifically pyspark code.

The use case here I am taking is of a Commerce company that has an ecommerce website as well as traditional retail stores. They want to analyse the online clickstream data to better understand their customers.

Clickstream data is data about how users interact with your ecommerce websites, what ads they click, what products they view, which pages they spend most time on. Behavioural data that can give you insights into your products and customers so you can better market to your customer base. Its important to start with the vision of any of these data projects. In my case, it will be to eventually develop ML models to provide product recommendations to my customers or to understand whether customers do not like any particular products, understand the churn rate.

We will use Dynamics products and customers data in data lake to do lookups and joins to enrich this raw data or bronze delta table and create more refined tables, or silver delta table. Finally do some aggregation and create a Gold delta table and do some basic analytics right within Databricks.

