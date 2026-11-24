An Excel project that takes a flat, denormalized retail sales table and splits it into a normalized relational structure (one fact table and three dimension tables). The tables are loaded into the Excel Data Model with Power Query, and a PivotTable is built on top of them.

The source data is a single wide table of 62,884 transaction lines across 31 columns. Every row repeats the customer, store and product details, which wastes space and makes updates error-prone. For example, changing a product price means editing thousands of rows.


Separates the repeated attributes into dedicated Customer, Product and Store tables.
Keeps a lean Transaction (fact) table that references them through ID keys.
Loads all four tables into the Excel Data Model via Power Query.
Builds a PivotTable from the model to show that the normalized structure still supports analysis.
Checks that nothing was lost or changed in the split.
