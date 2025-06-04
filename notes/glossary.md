# Glossary

- **ACID:** Atomicity, Consistency, Isolation, and Durability.
  - Problems solved by ACID:
    - Streamlined Data Append
    - Simplified Data Modification
    - Data Integrity Through Job Failures
    - Support for Real-time Operations
    - Efficient Historical Data Version Management

- **Data objects in Databricks:**
  - Metastore
  - Catalog
  - Schema (Database):
    - Table
    - View
    - Function
   
- **Liquid Clustering:**
  - No more partitions
  - Fast
  - Self-tuning
  - Incremental
  - Skew-resistant
  - Flexible
  - Better concurrency
  - Benefits:
    - Tables often filtered by high cardinality columns
    - Tables with significant skew in data distribution
    - Tables that grow quickly and require maintenance and tuning effort
    - Tables with access patterns that change over time
    - Tables where a typical partition key could leave the table with too many or too few partitions.
- **Deletion Vectors:**
  -  **Phothon** leverages deletion vector for predictive I/O updates, accelerating DELETE, MERGE and UPDATE operations.
 
-  **[Photon](https://docs.databricks.com/aws/en/compute/photon):** is a high-performance Databricks-native vectorized query engine that runs your SQL workloads and DataFrame API calls faster to reduce your total cost per workload.
-  **[Parquet](https://www.databricks.com/glossary/what-is-parquet):** Apache Parquet is an open source, column-oriented data file format designed for efficient data storage and retrieval. It provides efficient data compression and encoding schemes with enhanced performance to handle complex data in bulk.
- **Shallow Clone:** creates a copy of a table's metadata without copying the data files themselves. This means the new table references the original table's data. Shallow cloning is a cost-effective way to create copies for testing, experimentation, or short-lived use cases.
  - When to use it: 
    - When you need a temporary copy of a table for testing or development. 
    - When you want a cost-effective way to create a copy of a table. 
    - When you want to avoid copying large amounts of data. 
    - When you need to preserve the original table's data integrity.   
