# Final Project
## Amazon Product insights for Sales Estrategies.
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
## Project Structure:
## Conclusion
### Helpful resources to view
- [Dataset] (https://www.kaggle.com/datasets/asaniczka/amazon-products-dataset-2023-1-4m-products/data) : Source of the dataset.
- [SlideDeck] (https://drive.google.com/drive/u/0/folders/1Ep7Hfvq_3v8WH2T2-vXs1H0g7Ymklk_h) : Presentation slides of the project.
- [Tableau Dashboard] (https://public.tableau.com/app/profile/sabina.pacheco6424/viz/ProyectoAmazon/Dashboard1) : To make the presentation more engaging by visualizing the dashboard. 
