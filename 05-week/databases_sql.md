# Databases

**schema**: a set of rules for what goes in each table; often is the datatype that will be accepted for a given column
  - each *table* has a schema, which is a set of rules for the full table


Uber example:

Table: User table
- Primary Key: User ID
- User Name
- CC Number

Table: Driver table
- Primary Key: Driver ID
- Driver Name

Table: Ride table
- Primary Key: Ride ID
- Driver ID
- Ride Time
- Pickup Long
- Pickup Lat
- Pickup Location Entity
- Drop-off Longitude
- Drop-off Lat
- Drop-off Location Entity
- Miles
- Travel Time
- Fare

Table: Transactions
- Primary Key: CC Number
- Fare
- Miles
- Driver ID
- User ID
