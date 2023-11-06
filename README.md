# Amazon Product insights for Sales Estrategies. Final Project
<img src="https://crazylister.com/wp-content/uploads/2018/05/Amazon-Top-Sellers_FB.png" width = 800 alt="" title="" />

## Project Objective and Main questions
main problem: We are an e-commerce brand that is working as an amazon affiliate and we have all the Amazon products available to work with, how can we optimize sales strategies to maximize revenue by picking the star products and categories ?

**Key Questions:**

- What were the TOP 5 Best-selling categories last month?
- What is the most sold product of each one of these categories?
- What are the most sold products with the highest rating?
- Does the discount have any impact on the sales?
- Is it possible to predict future sales of a product based on this information?

## Dataset

| Column Name   | Description                                                                 |
| ------------- | --------------------------------------------------------------------------- |
| title         | Title of the product. (type:str)                                            |
| imgUrl        | Url of the product image. (type:str)                                        |
| productURL    | Url of the product. (type:str)                                              |
| stars         | Product rating. If 0, no ratings were found. (type:float)                   |
| reviews       |      Number of reviews. If 0, no reviews were found. (type:int)             |
| price         | Buy now price of the product. If 0, price was unavailable. (type:float, currency: USD)  
| listPrice     | Original price of the product before discount. If 0, no list price was found AKA, no discounts. (type:float, currency:     |
| category_id   | Use the amazon_categories.csv to find the actual category name. (type:int)  |
| isBestSeller  | Whether the product had the Amazon BestSeller status or not. (type:bool)    |
| boughtInLastMonth  | Units sells last month                                         |
| id     | id of the category. Has a foreign key relationship with "category_id" on amazon_products.csv (type:int)     |
| category_name | id of the category. Has a foreign key relationship with "category_id" on amazon_products.csv (type:int)
| Discount percentage    | We also calculated a discount percentage taking the price and listed price.   |
                                

## Tools Employed
- **Visualization**: Tableau
- **Exploratory Data Analysis (EDA)**: Python (Jupyter Notebook)
- **Machine Learning**: Python (Jupyter Notebook). Libraries : Matplotlib, Pandas,  seaborn, plotly.express. Correlation Matrix. 
## Project Structure:
1. **Import Libraries & Load Dataset**: Initialization of the data exploration and analysis journey.
2. **Dataset Overview**: A quick look into the data attributes.
3. **Data Normalization Cleaning**:
- We had 2 data frames: Categories and Products.
- In the dataframe categories we changed the column name ID to Category_id to normalize it with the other data frame’s column.
- We dropped 2 columns (Img URL and productURL) since they were irrelevant for the EDA
- We change column type from int to str since the id numbers correspond to category names. 
- We converted column names to Uppercase.
- Drop null values, and duplicated values
- Merge data frames into amazon_data.

4. **Exploratory Data Analysis (EDA)**: Delving deeper into the data to reveal insights.
5. **Correlation Matrix**
6. **Conclusion**: Summarizing findings and recommending future work.
## Conclusion
- Overall, most of the correlations in this matrix are very weak, indicating that the variables are not strongly related to each other.
- With this information, we can conclude that the best seller product performances are more influenced by the customer necesities based in other external factors not mentioned.
- The discount percentage doesn’t have a meaningful impact on the sales, since the top sold products are barely discounted or not at all.
- We can not acurately predict any future sales with this insights, however we indeed were able to  estimate the top products based on their sales perfomance and rating
### Helpful resources to view.

- [Dataset] (https://www.kaggle.com/datasets/asaniczka/amazon-products-dataset-2023-1-4m-products/data) : Source of the dataset.
- [SlideDeck] (https://drive.google.com/drive/u/0/folders/1Ep7Hfvq_3v8WH2T2-vXs1H0g7Ymklk_h) : Presentation slides of the project.
- [Tableau Dashboard] (https://public.tableau.com/app/profile/sabina.pacheco6424/viz/ProyectoAmazon/Dashboard1) : To make the presentation more engaging by visualizing the dashboard. 
