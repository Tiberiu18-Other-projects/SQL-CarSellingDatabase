**Project Theme**: 
Building the database for a car selling website, demonstrating the use through various SQL statements.

When a car is posted for sale, the ad must include:

- **Seller Details**:
  - Name
  - Surname
  - Phone
  - County of residence, etc.
  
- **Car Details**:
  - Brand (e.g., Peugeot, Opel, Porsche)
  - Model (e.g., 508 for Peugeot, Astra G for Opel, 911 for Porsche)
  - Manufacturing year
  - Type of fuel
  - Price

Also, there has to be an archive that holds all the ads that are no longer available (we assume that those cars have been sold) - kind of like an ad history.

**Entity Relationships**:

1. Between **Ads** and **Sellers**: 
   - 1:M (one to many) relationship.
   - An ad can be posted by only one seller, but a seller can have multiple ads.
   
2. Between **Sales History** and **Ads**: 
   - M:1 relationship.
   - In the history there can be multiple ads, but an ad can be posted only once in the history.

3. Between **Sellers** and **Counties**: 
   - M:1 relationship.
   - A seller can have residence in only one county, but in counties, there can be multiple sellers.


**Diagram**:
![image](https://github.com/Tiberiu18/SQL-CarSaleSimulator/assets/89936705/14790d35-2160-46b5-8cc2-e99ce205009a)
