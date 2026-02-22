# DP-203 Practice Questions with Answers

---

## 1. Hot vs Cool vs Archive tiers — when to choose
**Answer:** <span style="color:green">Hot for frequent access, Cool for infrequent (≥30 days storage), Archive for rarely accessed data (≥180 days, rehydration required)</span>

---

## 2. When to switch Databricks Standard → Premium
**Answer:** <span style="color:green">Switch when you need role-based access control, credential passthrough, table ACLs, or enterprise security features</span>

---

## 3. Reading Databricks cluster config JSON
**Answer:** <span style="color:green">Used to determine node type, autoscaling, runtime version, libraries, and Spark configuration</span>

---

## 4. Clustered columnstore + hash distribution column choice
**Answer:** <span style="color:green">Use business key or join key (ID column), not date column</span>

---

## 5. Star schema dimension surrogate key
**Answer:** <span style="color:green">Surrogate Key (SK) = artificial integer key, not business key</span>

---

## 6. When to choose SHIR (Self-hosted Integration Runtime)
**Answer:** <span style="color:green">When accessing on-prem data sources or private network resources</span>

---

## 7. Azure HDInsight purpose
**Answer:** <span style="color:green">Managed Hadoop ecosystem cluster for big data processing (Spark, Hive, Kafka, HBase)</span>

---

## 8. Synapse lifecycle vs soft delete vs retention vs Event Hub delete
**Answer:** <span style="color:green">Lifecycle = auto move/delete files, Soft delete = recoverable deletion, Retention = data kept for time window, Event Hub delete = purge events after retention expires</span>

---

## 9. Event Hub reference input vs stream input
**Answer:** <span style="color:green">Reference input = static lookup dataset, Stream input = real-time event stream</span>

---

## 10. Detect data skew
**Answer:** <span style="color:green">Check distribution row counts or skewed partition sizes</span>

---

## 11. Monitor ADF + Databricks jobs
**Answer:** <span style="color:green">Use ADF Monitor + Azure Monitor + Log Analytics + Databricks job logs</span>

---

## 12. Identify SCD Type 2 table
**Answer:** <span style="color:green">Presence of effective date, expiry date, and current flag columns</span>

---

## 13. Date dimension join with fact
**Answer:** <span style="color:green">Join on DateKey surrogate key</span>

---

## 14. Replicated dimension table
**Answer:** <span style="color:green">Small dimension tables replicated to all nodes for join performance</span>

---

## 15. SCD Type 2 update method
**Answer:** <span style="color:green">MERGE statement</span>

---

## 16. IoT folder structure best practice
**Answer:** <span style="color:green">Partition by region/year/month/day/device for parallel reads</span>

---

## 17. Find surrogate key
**Answer:** <span style="color:green">Identity or auto-increment column</span>

---

## 18. Remove old data efficiently
**Answer:** <span style="color:green">Partition switch</span>

---

## 19. Clustered index usage
**Answer:** <span style="color:green">Best for range queries and ordered scans</span>

---

## 20. Copy SQL → Synapse using R language
**Answer:** <span style="color:green">Use COPY INTO or Data Factory, not R</span>

---

## 21. Best storage format for IoT compression
**Answer:** <span style="color:green">Avro</span>

---

## 22. ADF Repo structure ARM templates location
**Answer:** <span style="color:green">Publish branch → ARM templates folder</span>

---

## 23. Real-time ingestion to ADLS
**Answer:** <span style="color:green">Databricks Auto Loader</span>

---

## 24. Event Hub retention setting
**Answer:** <span style="color:green">Defines how long events remain before automatic deletion</span>

---

## 25. Log monitoring query language
**Answer:** <span style="color:green">KQL (Kusto Query Language)</span>

---

## 26. Count tweets every 10 seconds
**Answer:** <span style="color:green">Tumbling window aggregation</span>

---

## 27. Count tweets every 10 sec in last sec
**Answer:** <span style="color:green">Hopping window</span>

---

## 28. ADLS authentication selection
**Answer:** <span style="color:green">Managed Identity for least maintenance</span>

---

## 29. Column-level security
**Answer:** <span style="color:green">CLS masks specific columns for users</span>

---

## 30. Row-level security
**Answer:** <span style="color:green">RLS filters rows based on user context</span>

---

## 31. Keep ADF logs 180 days
**Answer:** <span style="color:green">Send diagnostics to Log Analytics with retention configured</span>

---

## 32. Data Flow debug delay cause
**Answer:** <span style="color:green">Cluster spin-up time</span>

---

## 33. Identify failed pipeline
**Answer:** <span style="color:green">Check activity status = Failed in Monitor tab</span>

---

## 34. Synapse JSON read option for quotes
**Answer:** <span style="color:green">FIELDQUOTE parameter</span>

---

## 35. CROSS APPLY JSON parsing
**Answer:** <span style="color:green">OPENJSON</span>

---

## 36. Read tables listed in txt file in ADF
**Answer:** <span style="color:green">Lookup activity + ForEach loop</span>

---

## 37. Scala write command
**Answer:** <span style="color:green">saveAsTable</span>

---

## 38. Synapse Spark measurement unit
**Answer:** <span style="color:green">vCores</span>

---

## 39. Trigger type scenario-based
**Answer:** <span style="color:green">Depends: Schedule, Tumbling window, or Event-based</span>

---

## 40. Check table size distribution
**Answer:** <span style="color:green">DBCC PDW_SHOWSPACEUSED</span>

---

## 41. Streaming data read in Databricks
**Answer:** <span style="color:green">Structured Streaming readStream</span>

---

## 42. Transaction rollback pattern
**Answer:** <span style="color:green">BEGIN TRAN → TRY → COMMIT → CATCH → ROLLBACK</span>

---

## 43. SQL pool vs Spark pool choice
**Answer:** <span style="color:green">SQL pool = structured analytics; Spark = big data processing</span>

---

## 44. Append vs Update decision
**Answer:** <span style="color:green">Append for logs/streams, Update for dimensions</span>

---

## 45. JSON flatten query
**Answer:** <span style="color:green">EXPLODE / OPENJSON</span>

---

## 46. Least maintenance SAS option
**Answer:** <span style="color:green">Managed Identity instead of SAS</span>

---

## 47. Transparent Data Encryption purpose
**Answer:** <span style="color:green">Encrypt data at rest automatically</span>

---

## 48. Contoso case study decisions
**Answer:** <span style="color:green">Partition = date column, Distribution = hash on transaction ID, Table type = external for raw data, Range Right = correct boundary handling</span>

---
