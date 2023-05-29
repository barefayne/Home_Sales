# Home_Sales

In this challenge, you'll use your knowledge of SparkSQL to determine key metrics about home sales data. Then you'll use Spark to create temporary views, partition the data, cache and uncache a temporary table, and verify that the table has been uncached.

## Analysis:
1. What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places.

![Alternate image text](/Images/query_1.png)

2. What is the average price of a home for each year it was built that has three bedrooms and three bathrooms? Round off your answer to two decimal places.

![Alternate image text](/Images/query_2.png)

3. What is the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places.

![Alternate image text](/Images/query_3.png)

4. What is the "view" rating for homes costing more than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.

![Alternate image text](/Images/query_4.png)

### Run time comparisons:
* Uncached Runtime: 1.084960699081421 seconds
* Cached Runtime: 0.6035380363464355 seconds
* Runtime with the parquet DataFrame: 0.585641622543335 seconds

Based on the runtime comparison results, it is evident that utilizing caching or using a parquet DataFrame reduces the query runtime compared to running the query without any optimization.