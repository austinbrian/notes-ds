# Spatial Data and Analysis
----
### Correlated spatial data
- Spatial and temporal data are highly correlated, and that causes problems for making predictions most of the time
- Methods of working with spatial data:
  - Analysis - explain your dependence
  - Prediction
  - Adjustment - to "adjust" by space
  - Simulation
- Spatial data *Y(s)* are random variables, *s* is the spatial input, and the set of all *s* is *D*, the **spatial domain**

### Types of spatial data
- **Areal processes** - spatial domain is non-overlapping regions (e.g., states, zip codes)
- **Geostatistical process** - fixed spatial inputs that all measure a given thing, over a large area; goal is to understand what is happening with regard to a thing being measured (e.g., rainfall measurement stations)
- **Point-pattern process** - if spatial domain *D* is a collection of random points; goal is to understand where the thing being measured is happening (e.g., locations of terrorist attacks)

### Weight/Proximity/Distance Matrices
- Weight matrix *W* assesses how closely related two regions are - goal is to assign a weight that describes given region *i* to other regions *j*

### Moran's I Statistic
- Pass a vector of spatial data; small p-values allow you to conclude that spatial correlation exists, but doesn't provide information about the direction of the association


### Modeling strategy
- If you think that there is a spatial element to the data that will help in a decomposition:
  1. Try to estimate the trend by building a model on the spatial data (i.e., linear regression)
  2. For every observation *Y(s)* calculate the error that the model outputs
  3. Plot/examine the residuals and generate the covariance of the residuals

### Coding implementation
- Shapefiles: polygons that describe the outlines of geographic locations
- Convex hulls: outlines of geographic areas; simplifies the computational expense of locating an outline of an area.
