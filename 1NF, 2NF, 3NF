-- Pre Normalization Table --
CREATE TABLE Produce_RAW (
    Produce_ID INT PRIMARY KEY,
    Name VARCHAR(255),
    Email VARCHAR(255),
    Freshness_Indicator VARCHAR(255),
    Source_Location VARCHAR(255),
    Seasonal_Availability VARCHAR(255),
    Organic_Certification_Status VARCHAR(255),
    Category VARCHAR(50),
    Supplier_ID INT,
    Delivery_Option VARCHAR(100),
    Sustainability_Practices VARCHAR(255),
    Transaction VARCHAR(255),
    Subscription_Plans VARCHAR(255),
    Geolocation DECIMAL(9,6),
    Quality_Rating INT
);

--FIRST NORMAL FORM--
CREATE TABLE Produce (
    Produce_ID INT PRIMARY KEY,
    First_Name VARCHAR (255),
    Last_Name VARCHAR(255),
    Email VARCHAR (255),
    Freshness_Indicator VARCHAR(255),
    Source_Location VARCHAR(255),
    Seasonal_Availability VARCHAR(255),
    Organic_CertificationStatus VARCHAR(255),
    Category VARCHAR(255),
    Product VARCHAR(255),
    Supplier_ID INT,
    Delivery_Option VARCHAR(255),
    Sustainability_Practices VARCHAR(255),
    Transaction_Amount DECIMAL(10,2),
    Transaction_Date VARCHAR (255),
    Subscription_Plan VARCHAR(255),
    GeolocationLatitude DECIMAL(10,6),
    GeolocationLongitude DECIMAL(10,6),
    QualityRating DECIMAL(5,2)
);


--SECOND NORMAL FORM--
-- Produce Table
CREATE TABLE Produce (
    ProduceID INT PRIMARY KEY,
    FreshnessIndicator VARCHAR(255),
    SourceLocation VARCHAR(255),
    SeasonalAvailability VARCHAR(255),
    OrganicCertificationStatus VARCHAR(255),
    Category VARCHAR(255),
    Product VARCHAR(255),
    SustainabilityPractices VARCHAR(255),
    QualityRating INT,
    FOREIGN KEY (SupplierID) REFERENCES Supplier(SupplierID)
);




-- User Table
CREATE TABLE User_TABLE (
    UserID INT PRIMARY KEY,
    First_Name VARCHAR(255),
    Last_Name VARCHAR(255),
    Email VARCHAR(255),
    SubscriptionPlan VARCHAR(255)
);


-- Supplier Table
CREATE TABLE Supplier (
    SupplierID INT PRIMARY KEY,
    SupplierName VARCHAR(255)
);




-- Creating the Geolocation table
CREATE TABLE Geolocation (
    GeoID INT PRIMARY KEY,
    Latitude DECIMAL(9,6),
    Longitude DECIMAL(9,6),
    FOREIGN KEY (UserID) REFERENCES User_TABLE(UserID)
);

-- Transaction Table
CREATE TABLE Transaction (
    Transaction_ID INT PRIMARY KEY,
    Transaction_Amount DECIMAL(10,2),
    Delivery_Option VARCHAR(255),
    Transaction_Date DATE
);

-- THIRD NORMAL FORM--
-- Produce Table
CREATE TABLE Produce (
    ProduceID INT PRIMARY KEY,
    FreshnessIndicator VARCHAR(255),
    SourceLocation VARCHAR(255),
    SeasonalAvailability VARCHAR(255),
    OrganicCertificationStatus VARCHAR(255),
    SustainabilityPractices VARCHAR(255),
    QualityRating INT,
    FOREIGN KEY (SupplierID) REFERENCES Supplier(SupplierID)
);


-- User Table
CREATE TABLE User_TABLE (
    UserID INT PRIMARY KEY,
    First_Name VARCHAR(255),
    Last_Name VARCHAR(255),
    Email VARCHAR(255),
    SubscriptionPlan VARCHAR(255)
);


-- Supplier Table
CREATE TABLE Supplier (
    SupplierID INT PRIMARY KEY,
    SupplierName VARCHAR(255)
);




-- Creating the Geolocation table
CREATE TABLE Geolocation (
    GeoID INT PRIMARY KEY,
    Latitude DECIMAL(9,6),
    Longitude DECIMAL(9,6),
    FOREIGN KEY (UserID) REFERENCES User_TABLE(UserID)
);




-- Transaction Table
CREATE TABLE Transaction (
    Transaction_ID INT PRIMARY KEY,
    Transaction_Amount DECIMAL(10,2),
    Delivery_Option VARCHAR(255),
    Transaction_Date DECIMAL(10,2)
);


CREATE TABLE Category (
    CategoryID INT PRIMARY KEY,
    Category VARCHAR(255),
    Product VARCHAR(255)
);
