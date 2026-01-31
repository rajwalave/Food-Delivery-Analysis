# Food Delivery Data Analysis  
### Innomatics Research Labs – Advanced GenAI Internship (Entrance Test)

## Project Overview

This project focuses on combining and analyzing real-world food delivery data provided in **multiple formats** (CSV, JSON, and SQL).  
The objective is to create a **single source of truth dataset** and perform analytical insights on user behavior, revenue trends, and restaurant performance.

## Datasets Used

The project uses the following datasets:

| File Name | Format | Description |
|---------|--------|------------|
| `orders.csv` | CSV | Transactional order data |
| `users.json` | JSON | User master data |
| `restaurants.sql` | SQL | Restaurant master data (cuisine, rating) |

## Data Integration Process

1. Loaded **CSV** data using Pandas  
2. Loaded **JSON** data using Pandas  
3. Imported **SQL** data into SQLite and read it into Pandas  
4. Merged datasets using **LEFT JOINs** to retain all orders  

### Join Keys:
- `orders.user_id` → `users.user_id`
- `orders.restaurant_id` → `restaurants.restaurant_id`

## Final Output

- **Final Dataset:** `final_food_delivery_dataset.csv`
- **Total Records:** 10,000 rows
- This dataset serves as the **only source of truth** for all analyses.

## Analysis Performed

The following insights were derived from the final dataset:

- City-wise revenue analysis
- Cuisine-wise performance
- Gold vs Regular membership impact
- Average order value analysis
- Rating-based revenue contribution
- Seasonal and quarterly revenue trends
- User spending behavior

## Technologies Used

- Python 
- Pandas
- SQLite
- Jupyter Notebook

## Key Learning Outcomes

- Handling multi-format datasets
- Performing joins across heterogeneous data sources
- Creating production-ready analytical datasets
- Applying Pandas for real-world business analysis

