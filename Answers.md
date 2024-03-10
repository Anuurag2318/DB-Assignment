1. Explain the relationship between the "Product" and "Product_Category" entities from the above diagram.

Answer- The relationship between the "Product" and "Product_Category" entities in the diagram is one-to-many. In the database, this relationship is represented by a foreign key i.e. in the Product table, the category_id column is a foreign key that references the primary key of the Product_Category table. This means that each product must be assigned a category, but a category can have many products. For Example, a product can be a "T-shirt"  and can belong to the categories "Clothing" and "Activewear".

2. How could you ensure that each product in the "Product" table has a valid category assigned to it?

Answer- To ensure that each product in the "Product" table has a valid category assigned to it, I can use foreign key constraints. I can set up a foreign key constraint on the "category_id" column in the "Product" table that references the "id" column in the "Product_Category" table. This constraint will ensure that every "category_id" in the "Product" table corresponds to a valid "id" in the "Product_Category" table.
For Example: If a product is assigned a "category_id" that doesn’t exist in the "Product_Category" table, the database will return an error and prevent the operation.
