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
