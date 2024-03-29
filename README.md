## Background
The purpose of this project was to use Machine learning models to cast a prediction for the future spending in the residential sector on electricity for the year 2021.
Their results will then be compared and a report will be drafted.


EIA's State Energy Data System (SEDS) is a comprehensive data set that consists of annual time series estimates of state-level energy use by major economic sectors, energy production and and State-level energy price and expenditure data. The system provides data back from 1960. Data are presented in physical units, BTUs, and dollars. While some SEDS data series come directly from surveys conducted by EIA, many are estimated using other available information. These estimations are necessary for the compilation of "total energy" estimates.

Useful Links:

The main website: https://catalog.data.gov/dataset/state-energy-data-system-seds

Additional information: https://www.eia.gov/state/seds/

Codes and descriptions: https://www.eia.gov/state/seds/CDF/Codes_and_Descriptions.xlsx


From the State Data energy System description sheets: \
The MSNs are five-character codes, most of which are structured as follows:
First and second characters - describes an energy source (for example, NG for natural gas, MG for motor gasoline)
Third and fourth characters - describes an energy sector or an energy activity (for example, RC for residential consumption, PR for production)
Fifth character - describes a type of data (for example, P for data in physical unit, B for data in billion Btu and D is for dollars per million BTU)


The aim of this project is to predict the Primary average price in the residential sector for the year 2021 based on residential sector features.


When loaded the file contains several columns: \
`Data_Status` - A Code \
`MSN` - A 5 letter combination to signify energy source, sector and unit of data.\
Units for each category are given below.\
Please see :https://www.eia.gov/state/seds/CDF/Codes_and_Descriptions.xlsx for a full description of each category. 
*	Million Btu per short ton
*	Billion Btu
*	Dollars per million Btu
*	Thousand short tons
*	Million dollars
*	Thousand barrels

`StateCode` Two letter state abbreviation \
`Year` YYYY-MM-DD \
`Data` Numerical - associated with MSN 


Models tested so far:

* Linear regression Model 
* Support Vector Regression Machine 
* K Neighbors regressor
* Neural Network model
* Stochastic Gradient Descent

Model Results So far:

The linear model performed very well. With a prediction accuracy of 100%. 


The `MAE` was 0.03267136765242417\
The `MSE` was 0.003015192149111796\
The `Explained variance` was 0.999999999844917\
The $ R^2 $ was 0.9999999998350794


The SVR performed very well. With a prediction accuracy of 100%.

The `MAE` was 0.5021485094357804\
The `MSE` was 0.6832135549229309\
The `Explained variance` was 0.9999999633196209\
The $ R^2 $ was 0.999999962630569



The SGDR performed very well. With a prediction accuracy of 100%.

The `MAE` was 0.9834673843854801\
The `MSE` was 1.5266552927792496\
The `Explained variance` was 0.9999999450342941\
The $ R^2 $ was 0.9999999164972077

The k_neighbors performed very well. With a prediction accuracy of 100%.

The `MAE` was 0.9834673843854801\
The `MSE` was 1.5266552927792496\
The `Explained variance` was 0.9999999450342941\
The $ R^2 $ was 0.9999999164972077

The Neural Network Model performed very well. With a prediction accuracy of 100%.\
The `MAE` was 0.032168487841461764\
The `MSE` was 0.0030038938705200698\
The `Explained variance` was 0.9999999998453984\
The $ R^2 $ was 0.9999999998356973


The Neural Network Model performed very well. With a prediction accuracy of 100%.

The `MAE` was 0.032168487841461764\
The `MSE` was 0.0030038938705200698\
The `Explained variance` was 0.9999999998453984\
The $ R^2 $ was 0.9999999998356973
