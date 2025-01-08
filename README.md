# Airbnb-Listing-EDA-New-York-2024-Data-Analysis-Project

![image](https://github.com/user-attachments/assets/1748626e-039e-49bc-a590-b14353acd70a)

# Project Overview 
The project involves performing an Exploratory Data Analysis (EDA) on New York Airbnb data to derive insights into rental trends and patterns. Pandas, NumPy, Matplotlib, and Seaborn are the primary libraries used for cleaning, analyzing, and visualizing data.

# Objective
The goal of this project is to:
1.	Analyse room types, prices, and availability across different neighborhoods.
2.	Understand host behavior and listing patterns.
3.	Detect potential outliers in prices.
4.	Provide recommendations for guests and hosts based on insights.

# Dataset
The dataset contains 20,765 entries and 22 features, including:
•	id: Unique identifier for each listing
•	name: Title of the Airbnb listing
•	host_name: Name of the host
•	neighborhood_group: Group (borough) where the listing is located
•	latitude/longitude: Geolocation of listings
•	price: Nightly rental price
•	room_type: Type of accommodation (e.g., entire home, private room)
•	reviews_per_month: Average monthly reviews for the listing
•	availability_365: Number of available days in the year

# Steps and Workflow
-- Importing All Dependencies


We import essential Python libraries such as NumPy, pandas, Matplotlib, and Seaborn. 


These libraries aid in tasks like analyzing duplicate rows, handling missing data, changing data types, and uncovering various insights.


Key insights include locality and review dependency, neighborhood group patterns, availability trends, price distribution, geographical distribution, and review behavior.

![image](https://github.com/user-attachments/assets/bf564c2e-b69a-41a8-8371-9efcddf01d69)

-- Loading Dataset and Statistical Information about data  
We imported the dataset, a dataset.csv file obtained from the Kaggle website. 

The dataset was uploaded to Google Collaboratory, where we ran the commands shown in the screenshots below.


We analyzed the Airbnb dataset to extract overall details and described its statistical information. 



![image](https://github.com/user-attachments/assets/7f4aa86e-1cca-4fc2-8f53-7f927e12c3ab)


![image](https://github.com/user-attachments/assets/03ad9597-93be-479c-871e-bbb2ec6d32ed)

![image](https://github.com/user-attachments/assets/b4c25ab1-b499-4850-b1b4-24a780bef881)


# Data Cleaning 


•	Handle missing data:


price, neighborhood, beds, latitude, longitude, room_type, minimum_nights, number_of_reviews, last_review, reviews_per_month, 

calculated_hosted_listing_count, availability_365, numbers-of_reviews_itm columns had null values, 

dropping all missing values rows and Dealing with Duplicate Rows. 


![image](https://github.com/user-attachments/assets/3c588d73-5676-4258-ae9a-aa668af1069a)


![image](https://github.com/user-attachments/assets/57d9e064-6d4a-4895-bee3-ba2b2889bf11)


![image](https://github.com/user-attachments/assets/2cfa25d1-a058-4dff-97fb-22a42885439f)


![image](https://github.com/user-attachments/assets/33efe96f-cadf-4796-9d00-0dbacb31a421)



•	Fix data types: Converted datatypes like id and host_id to a float64 object.


![image](https://github.com/user-attachments/assets/bbabec96-c2a8-4bff-9bd9-074a0fc53d94)



•	Locality and Review Dependency:


 Analyse no_of_reviews, price, and neighbourhood_group for showing locality and Review Dependency using Scatterplot.

 

 ![image](https://github.com/user-attachments/assets/1c4d8cf0-abc7-4bd3-b049-073f61467da8)

•	Neighborhood group insights:
    o	Analyzed price variations by boroughs.
    
    o	Manhattan had the highest average prices using bar plots.
    

![image](https://github.com/user-attachments/assets/cd4a0298-386e-4e8b-93ce-3338836181c4)


•	Availability trends:
    o	Used heatmaps to show correlations among price, availability_365, number_of_reviews, beds, latitude ,longitude, minimum_nights and reviews_per_month.

![image](https://github.com/user-attachments/assets/4af77632-17f9-44b1-a329-e3d88c029381)


•	Price distribution:
  o	Used histograms to show the distribution of prices.
  o	Majority of the listings were priced between $0 - $1500.

![image](https://github.com/user-attachments/assets/facac8a7-cb57-47dc-a50b-69045186ed05)


•	Geographical Distribution of Airbnb Listing:
    o	Analysed distribution with multiple listings using scatterplot to identify listings like Private Room, Entire Home/Apt, Hotel Room, and Shared Room.

![image](https://github.com/user-attachments/assets/5f089489-b8b8-4537-b281-51db1bfd630d)

•	Review or Host behavior:
    o	Used pair plots to show relationships between a number of reviews, price, and availability.

![image](https://github.com/user-attachments/assets/0cedee63-1576-4fd8-9050-b4ca6093f034)

# Data Visualization

  •	Pairplot: To see correlations among price, availability, and number of reviews.
  •	Heatmap: Showing correlations among numerical features.
  •	Histograms and Boxplots: To detect outliers in price.
  •	Bar Charts: Displaying room types and neighborhood group distributions.

# Key Findings and Insights
1.	Price Trends:

    o	Manhattan has the most expensive listings, followed by Brooklyn.

    o	Entire homes/apartments cost significantly more than private or shared rooms.

   
2.	Room Type Distribution:

    o	Entire homes/apartments are the most common, but private rooms offer budget-friendly options.

   
3.	Outliers in Price:
    o	Few listings priced greater than 1500 were detected, indicating the need to filter such extreme values.

   
4.	Availability Patterns:
    o	Listings with high availability tend to have lower prices and more reviews, likely due to better guest experience.

   
5.	Host Behaviour:
    o	Some hosts manage multiple listings, indicating a trend toward professional hosting.
  	

# Recommendations

•	For Guests:

    o	Look for listings with high availability and good reviews for a better experience.
    
    o	Private rooms in Brooklyn offer affordable stays compared to Manhattan.

    
•	For Hosts:

    o	Improve availability and review response rates to attract more bookings.

    
    o	Manage pricing effectively to compete within the borough's market.

    

# Conclusion

This project offers valuable insights into the New York Airbnb market, helping both guests and hosts make informed decisions.

By using EDA techniques, we identified key trends and developed actionable recommendations. 

Future improvements can involve advanced analytics and predictive modeling to further enhance the findings.




























