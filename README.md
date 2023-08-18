# Project description

For production company "GlavRosGosNeft". Need to decide where to drill a new well.

Provided oil samples from three regions: each has 10,000 fields where they have measured the quality of the oil and the amount of oil reserves. Build a machine learning model to help determine the region where production will yield the highest profit. Analyze the possible profits and risks using the *Bootstrap.* technique.

Steps for selecting a location:

- In the selected region, look for deposits and determine feature values for each;
- Build a model and estimate the amount of reserves;
- Select the fields with the highest estimated values. The number of fields depends on the company's budget and the cost of developing one well;
- Profit is equal to the total profit of the selected fields.

Profit prediction of a bunch oil well

## Data description
The exploration data of the three regions are in the files:
 * geo_data_0.csv. Download dataset
 * geo_data_1.csv. Download dataset
 * geo_data_2.csv. Download dataset
 * id - unique well identifier;
 * f0, f1, f2 - three point features (it does not matter what they mean, but the features themselves are significant);
 * product - volume of reserves in the well (thousand barrels).



**Problem conditions:**
 * Only linear regression is suitable for model training (the others are not predictable enough).
 * When exploring the region, 500 points are investigated, from which 200 best points are selected for profit calculation.
 * The budget for well development in the region is 10 billion rubles.
 * One barrel of raw materials generates 450 rubles of income. The income from each unit of the product is 450 thousand rubles, because the volume is specified in thousands of barrels.
 * After risk assessment, only those regions should be left where the probability of losses is less than 2.5%. The region with the highest average profit is selected among them.

Data are synthetic: contract details and field characteristics are not disclosed.