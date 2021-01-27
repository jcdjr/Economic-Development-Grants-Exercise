# Exploring Data on Economic Development Grants in TN

**Counting, Aliasing, Aggregating, & Slicing**

1. How many counties are represented in the ecd table? 

2. How many companies did not have Economic Development grants (ed)? Alias as ed_companies. 

3. What is the total capital_investment, in millions, when there is an fjtap? Call the column fjtap_cap_invest_mil. 

4. What is the average number of new jobs for each county_tier? 

5. How many companies are LLCs (combine COUNT() and DISTINCT())? Call this value llc_companies.

**Case Statements**

6. Using the population table in the ecd database, write a query that selects the county, 2017 population, and uses a case statement to characterize the 2017 population (pop_category) according to the following business rule: Greater than or equal to 500,000 - high population Between 100,000 and 500,000 - medium population Less than or equal to 100,000 - low population 

7. Using the ecd table in the ecd database, write a query that selects the company, landed date, number of new jobs, and a case statement to classify observations (rows) in the table where the project type is ‘New Startup’ according to the following business rule: Fewer than 50 new jobs – small startup Between 50 and 100 new jobs – midsize startup More than 100 new jobs – large startup 

8. Using the population table in the ecd database, write a query that uses a case statement to find the total population for 2010 and 2017. Call these Total_Pop_2010 and Total_Pop_2017.

**Simple Subqueries**

9. Write a subquery in the WHERE clause to select the top 5 capital investment amounts from the ecd table. Be sure to exclude NULL capital investments in the subquery. Next write an outer query to return the company, landed date, county, and capital investment for the top 5 investment amounts.

10. Use a subquery in the FROM section to find observations in county tier 4 with capital investment greater than $10,000,000 in the ecd database. Remember to alias your subquery! Next write an outer query to find the average number of new jobs and the average amount of total grants where an economic development grant is included in the total for this group.

**Partition**

11. For each Tennessee county in the population table in the ecd database: a. create a partition to find the maximum population(max_pop) values in the table. b. Also find the minimum population (min_pop) for each county.
