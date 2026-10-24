SELECT 
    SUM(Total_Sales) AS Total_Sales,
    SUM(Profit) AS Total_Profit
FROM sales_performance_data;


SELECT 
    Customer_ID, 
    Customer_Name, 
    SUM(Total_Sales) AS Total_Sales
FROM sales_performance_data
GROUP BY Customer_ID, Customer_Name
ORDER BY Total_Sales DESC
LIMIT 1;


SELECT 
    Category, 
    SUM(Total_Sales) AS Total_Sales
FROM sales_performance_data
GROUP BY Category
ORDER BY Total_Sales DESC;


SELECT 
    Customer_ID, 
    Customer_Name, 
    SUM(Total_Sales) AS Total_Sales
FROM sales_performance_data
GROUP BY Customer_ID, Customer_Name
ORDER BY Total_Sales DESC;


SELECT COUNT(*) AS Total_Customer FROM sales_performance_data


SELECT MAX(Salary) AS HighestSalary FROM sales_performance_data;


SELECT MIN(Salary) AS LowestSalary FROM sales_performance_data;


SELECT AVG(Salary) AS AverageSalary FROM sales_performance_data;
