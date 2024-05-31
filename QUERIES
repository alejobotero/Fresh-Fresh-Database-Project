--Retrieve all available produce listings along with their suppliers' information:
SELECT Produce_ID, Freshness_Indicator, Source_Location, Seasonal_Availability,
       Organic_CertificationStatus, Sustainability_Practices, QualityRating,
       SupplierName
FROM Produce
JOIN Supplier ON SupplierID = SupplierID;


--Retrieve transactions made on a specific date
SELECT *
FROM Transaction
WHERE Transaction_Date = '2024-01-05';


--Get the average quality rating of produce sold by each supplier:
SELECT SupplierID, SupplierName, AVG(QualityRating) AS AverageQualityRating
FROM Supplier
JOIN Produce ON SupplierID = SupplierID
GROUP BY SupplierID, SupplierName;


--Find users who have a subscription plan:
SELECT UserID, First_Name, Last_Name, Email
FROM User_TABLE
WHERE SubscriptionPlan = 'TRUE';


--Filter products based on location, organic certification, and product type:
SELECT *
FROM Produce
WHERE SourceLocation = 'Hunter College' AND OrganicCertificationStatus = 'TRUE' AND Category = 'Vegetables';


--Retrieve the latitude and longitude of all users for geolocation:
SELECT g.GeoID, g.Latitude, g.Longitude, u.First_Name, u.Last_Name
FROM Geolocation g
JOIN User_TABLE u ON g.UserID = u.UserID;
