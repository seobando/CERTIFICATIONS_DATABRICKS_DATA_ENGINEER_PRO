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
- ** Deletion Vectors:**
  -  **Phothon** leverages deletion vector for predictive I/O updates, accelerating DELETE, MERGE and UPDATE operations.
 
-  **[Photon](https://docs.databricks.com/aws/en/compute/photon):** is a high-performance Databricks-native vectorized query engine that runs your SQL workloads and DataFrame API calls faster to reduce your total cost per workload.

-  **[Parquet](https://www.databricks.com/glossary/what-is-parquet):** Apache Parquet is an open source, column-oriented data file format designed for efficient data storage and retrieval. It provides efficient data compression and encoding schemes with enhanced performance to handle complex data in bulk. 
