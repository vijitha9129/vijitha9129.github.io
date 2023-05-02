## Portfolio

---

### ML Projects

[Last Mile Delivery](/sample_page)
<p> : I did a POC for one of our clients on Last mile Delivery. This is for a postal company which delivers its packages everyday. There are certain vehicle sizes assigned to each of its routes and the end goal is to optimize the vehicle utilization and eventually reduce the carbon foorprint of the delivery service. So we had to determine the vehicles that are over utilized or underutilized and re-assign the routes for optimal usage. For example, if the cubic volume of the package size is 100 cubic feet then a vehicle which is close to this capacity has to be chosen and a bigger vehicle might be a wrong choice as it will be over utilized. Bigger vehicle means extra usage of fuel and hence carbon foot print is increased. 
Solution: We proposed two solutions for this problem. We had history of data with route_id’s, assigned_vehicle, vehicle_capacity and parcel_capacity. 
Approach 1: The first solution is to extract a new feature to determine the optimal vehicle based on the parcel_capacity and the vehicle capacity and utilization_level (which is another new feature created). Utlization level is calculated as percentage of the vehicle space used. If less than 50 percent of the vehicle space is utilized then it is under utilized and if more than 80 percent is used, vehicle space is over utilized. Other wise the vehicle is optimally used. Then based on the new feature which is optimal_vehicle_id, an algorthim is trained on new_id , parcel_capacity and route_id so that the algorithm will predict a new optimal vehicle based on the route_id and parcel_capacity. Decision tree and Random forest were used and Random forest gave us more accuracy. 
Approach 2: Using timeseries models to forecast the parcel_capacity by taking the year, month and day for the time and parcel_capacity as another feature to input to the models. The prediction was done for the next 10 days and then assign a vehicle based on the forecasted parcel capacity. I used XGboost and Sarima models to forecast the capacity of the parcels based on the history data. The data has seasonality component as the trend of the parcels increased during the holiday season. Hence Sarima model perfomed better in this case. 
My Responsibilities: I was the only person who worked on this project end to end. Hence I did exploratory data analysis, Feature Engineering, normalizing the data and then train and test the data by feeding it to ML models
Tech Stack: Python – Pandas, Numpy, Scikit-Learn, Matplotlib, Seaborn, AWS Sagemaker, EC2
<p/>

---
[Project 2 Title](/pdf/sample_presentation.pdf)
<img src="images/dummy_thumbnail.jpg?raw=true"/>

---
[Project 3 Title](http://example.com/)
<img src="images/dummy_thumbnail.jpg?raw=true"/>

---

### Category Name 2

- [Project 1 Title](http://example.com/)
- [Project 2 Title](http://example.com/)
- [Project 3 Title](http://example.com/)
- [Project 4 Title](http://example.com/)
- [Project 5 Title](http://example.com/)

---




---
<p style="font-size:11px">Page template forked from <a href="https://github.com/evanca/quick-portfolio">evanca</a></p>
<!-- Remove above link if you don't want to attibute -->
