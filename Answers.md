# Answers to Database Assignment

## Question 1: Explain the relationship between the "Product" and "Product_Category" entities from the above diagram.

The relationship between the "Product" and "Product_Category" entities is a many-to-one relationship. This means that many products can belong to one category, but each product can only belong to one category at a time. This relationship is established through the `category_id` foreign key in the "Product" table, which references the primary key `id` in the "Product_Category" table.

## Question 2: How could you ensure that each product in the "Product" table has a valid category assigned to it?

To ensure that each product in the "Product" table has a valid category assigned to it, you can use a foreign key constraint. In the "Product" table, the `category_id` column should be defined as a foreign key referencing the `id` column in the "Product_Category" table. By doing this, the database will enforce referential integrity, ensuring that only valid category IDs can be inserted into the `category_id` column of the "Product" table.
