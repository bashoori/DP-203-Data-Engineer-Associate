# DP-203-Data-Engineer-Associate

DP-203 Azure Data Engineer Associate Sample Questions List :

1. When designing a multi-region Cosmos DB account with session consistency, which configuration ensures the lowest RTO during regional failover without data loss?
Single write region with manual failover

Multi-region writes with automatic failover

Single write region with service-managed failover

Multi-region writes with manual failover

2. When implementing cross-tenant data sharing via Azure Data Share, what ensures data residency compliance?
Private endpoint configuration

Source-defined export settings

Snapshot execution region

Recipient storage location

3. For a Parquet dataset in ADLS Gen2 receiving 5 TB/hour streaming IoT data, which partitioning strategy optimizes query performance for time-range filters?
Partition by device ID Hive-style

Hourly partition on event timestamp

Round-robin partitioning

Hash partitioning on sensor type

4. Which Blob Storage feature reduces latency for Spark on Synapse accessing hot-tier data?
Archive tier migration

Premium block blobs

Immutable storage

Object replication

5. In Synapse serverless SQL pool, what happens when querying a Delta Lake table with ZORDER applied on the "customer_id" column?
Automatic statistics update in metastore

Predicate pushdown to storage layer

Data skipping via zone maps

In-memory caching of frequent segments

6. In a Cosmos DB analytical store, what determines the partition key for auto-synced data?
Inherited from transactional store logical partition key

Configurable during Synapse link setup

Automatic hash distribution

Fixed by Azure at container level

7. Which Blob Storage feature reduces egress costs by 50% for analytics workloads accessing cold-tier data in North Europe from a Synapse cluster in West Europe?
Geo-redundant storage (GRS)

Azure CDN integration

Object replication to West Europe

RA-GRS read access

8. Which command forces materialization of a Spark dataframe before writing to Delta Lake?
.cache()

.checkpoint()

.persist()

.materialize()

9. When implementing columnstore indexes in Synapse dedicated SQL pool, which compression technique dynamically adapts to data patterns without manual intervention?
PAGE compression

Reorganize index with COMPRESS_ALL option

Automatic adaptive compression

Rowgroup-level dictionary encoding

10. What happens when you enable "Version Level Immutability" on an ADLS Gen2 container?
All blob versions become WORM-protected

Only current version is immutable

Auto-deletes versions after retention period

Disables soft delete functionality

11. What's the primary advantage of using Delta Lake's `OPTIMIZE ZORDER BY` command on a timestamp column in ADLS Gen2?
Reduces storage footprint through compression

Accelerates point-in-time queries via data clustering

Enables cross-region replication for disaster recovery

Automatically partitions data into hourly chunks

12. For Synapse serverless querying CSV files, which configuration avoids schema inference errors?
OPENROWSET with explicit schema

CETAS with inferred types

Automatic schema detection

Schema drift settings

13. For a Polybase query loading 10TB from Blob Storage to Synapse, which credential configuration provides most secure access?
Shared Access Signature (SAS) token

Storage account key

Managed Identity

Azure AD user credentials

14. Which Cosmos DB feature reduces RU consumption for point reads by 80%?
Optimistic concurrency control

Session consistency

Direct TCP mode

Point read API

15. Which Cosmos DB indexing policy optimizes storage costs for an IoT telemetry system querying only by deviceId and timestamp?
Composite index on (deviceId, timestamp)

Spatial index on geolocation fields

Full range indexing on all properties

No indexing with manual queries

16. What's the impact of setting `spark.sql.parquet.mergeSchema=true` in Delta Lake?
Auto-resolves schema conflicts during writes

Enables schema evolution tracking

Forces schema validation on read

Disables partition discovery

17. When implementing column-level security in Synapse dedicated SQL pool, which feature prevents unauthorized users from viewing masked data?
Dynamic Data Masking policies

Row-Level Security filters

Transparent Data Encryption

Always Encrypted with secure enclaves

18. Which authentication method allows cross-tenant Synapse to ADLS access without secret sharing?
Service principal with client secret

Managed identity federation

SAS token delegation

Access key passthrough

19. What's the effect of enabling hierarchical namespace on an existing Blob Storage account containing 50TB of Parquet files?
Automatic conversion to Delta Lake format

Loss of access tier settings for existing blobs

Immediate 40% storage cost reduction

POSIX-compliant directory operations

20. When using Change Feed in Cosmos DB for incremental loads, what ensures exactly-once processing?
Session token persistence

ETag checkpointing

Lease container partitioning

Change Feed processor

21. Which compression algorithm provides the best query performance for analytical workloads in Synapse serverless SQL pools?
GZIP

SNAPPY

LZO

BZIP2

22. Which Synapse workload management feature prevents runaway queries?
Resource classes

Workload groups

Query importance

Request limits

23. For a slowly changing dimension in Synapse, which table distribution strategy minimizes data movement during SCD Type 2 merges?
Hash-distributed on business key

Round-robin distribution

Replicated table

Range-distributed on timestamp

24. What's the purpose of V-Order in Parquet writes from Synapse Spark?
Enhanced compression dictionary sorting

Vectorized execution optimization

Z-Order equivalent for single columns

Page-level checksum validation

25. For GDPR data subject requests, which ADLS feature automates PII deletion?
Lifecycle management rules

Immutable storage holds

Object tagging with filters

Access policy conditions

26. Which feature enables schema enforcement when streaming into Delta Lake from Azure Event Hubs?
Auto Loader with schema inference

Delta Lake schema validation

Event Hubs schema registry

Stream Analytics JSON parser

27. When configuring Azure Data Lake Analytics (legacy), what determines parallel job execution?
AU allocation per job

Degree of parallelism setting

Vertex count in U-SQL script

Data partitioning scheme

28. What is the primary purpose of materialized views in Azure Synapse serverless SQL pool?
Pre-aggregate frequently queried data

Automatically index foreign keys

Replace fact table partitioning

Enable cross-database queries

29. Which feature allows querying Parquet files in Blob Storage without data movement?
Synapse serverless SQL pool

Data Lake Analytics

PolyBase in Azure SQL DB

Databricks Runtime

30. When implementing a medallion architecture in ADLS Gen2, which pattern describes the raw data zone?
Bronze: Unmodified source data

Silver: Validated and enriched data

Gold: Business-aggregated data

Platinum: ML-optimized data

31. For GDPR compliance, which ADLS Gen2 feature automates PII data deletion?
Lifecycle management + blob index tags

Immutable storage policies

Soft delete retention

Customer-managed keys

32. Which Cosmos DB setting reduces storage costs by 70% for infrequently accessed metadata?
Analytical TTL

Autoscale throughput

Standard provisioning

Serverless capacity mode

33. What is the primary benefit of Z-order indexing in Delta Lake?
Improves compression ratios

Enables ACID transactions

Accelerates multi-column predicates

Reduces VACUUM costs

34. For a Synapse pipeline loading 100GB/hour into a dedicated SQL pool, which copy method minimizes resource contention?
PolyBase with external tables

COPY INTO statement

SSIS package execution

Bulk Insert T-SQL command

35. Which authentication method should be deprecated for Blob Storage access in 2025?
Shared Key authorization

Azure AD service principal

SAS tokens with stored policies

Managed identity

36. What is the effect of enabling accelerated networking on an Azure VM hosting a SQL Server instance?
Reduces latency between compute and Premium SSDs

Enables RDMA for Storage Spaces Direct

Bypasses hypervisor for network traffic

Increases throughput to Azure NetApp Files

37. When using Synapse Spark to process Delta Lake tables, what does `VACUUM RETAIN 0 HOURS` do?
Removes all historical versions

Compacts small files

Updates statistics

Optimizes Z-order

38. Which Blob Storage access tier is optimized for write-once-read-never workloads?
Hot

Cool

Cold

Archive

39. Which Cosmos DB API provides MongoDB 4.2 wire protocol compatibility?
Core (SQL) API

MongoDB API

Cassandra API

Gremlin API

Overall explanation

40. When using Synapse Link for Cosmos DB, what synchronizes data between transactional and analytical stores?
Change Feed processor

Automatic TTL replication

Azure Data Factory pipeline

Near-real-time ETL job

41. For time-series IoT data in ADLS Gen2, which file format minimizes storage costs?
CSV with GZIP

Avro with DEFLATE

Parquet with SNAPPY

ORC with ZLIB

42. Which compression type is not supported natively by Delta Lake?
ZSTD

LZ4

SNAPPY

GZIP

43. What happens when you enable read-access geo-redundant storage (RA-GRS) on Blob Storage?
Secondary region becomes readable

Automatic failover to secondary region

Triple replication in primary region

Object versioning enabled

44. For a slowly changing dimension table in Synapse, which distribution type minimizes data movement during updates?
Hash-distributed

Round-robin

Replicated

Range-distributed

45. Which Synapse security feature encrypts data at rest using customer-controlled keys?
Transparent Data Encryption (TDE)

Always Encrypted

Dynamic Data Masking

Row-Level Security

46. What does enabling hierarchical namespace on Blob Storage enable?
POSIX-compliant access control lists

Automatic file format conversion

Geo-zone-redundant storage

Object-level immutability

47. When implementing Change Data Capture (CDC) for Azure SQL DB to Synapse, which tool provides lowest latency?
Azure Data Factory mapping data flows

Kafka Connect with Debezium

SQL Server Integration Services

Azure Databricks Auto Loader

48. Which Cosmos DB consistency level provides linearizability at the cost of higher latency?
Strong

Bounded staleness

Session

Consistent prefix

49. Which Cosmos DB feature automatically scales throughput based on demand?
Autoscale provisioned throughput

Serverless capacity mode

Manual RU adjustment

Partition key splitting

50. For a star schema in Synapse dedicated SQL pool, which fact table distribution strategy optimizes query performance?
Hash-distributed on fact key

Round-robin

Replicated

Hash-distributed on join key

