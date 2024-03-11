## Answer 1
The realtionship between "Product" and "Product_Category" is one-to-many. One product can belong to one category but a category can have many products because in the schema therre is a key called category_id in the Product table. A foreign key is a column in a table that refrences the primary key of another table. Here, the category_id column in the Product table refrenbces the id column in the Product_Category table.

## Answer 2
There are several ways to ensure every product in the Product table has a vaild category assigned:

1. Foreign Key Constraint: The database keeps a foreign key constraint on the "category_id", must exist as a primary key in "Product_Category" table.

2. Validation: When a new product is added, the application can validate the chosen category before saving the product.
