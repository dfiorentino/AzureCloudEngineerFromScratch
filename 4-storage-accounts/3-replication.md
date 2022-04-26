# Redundancy and Disaster Recovery

**Redundancy in the primary region:**

The data in an Azure Storage is replicated three times in the same region. In this case Azure offers two type options:

<strong>Locally Redundant Storage (LRS):</strong> copies your data synchronously three times within a single physical location in the primary region. 

- LRS provides a SLA 99.999999999% (11 nines) over a year
- Lowest-cost redundancy option
- Not recommended for high availability or durability 

<strong>Zone Redundant Storage (ZRS):</strong> copies your data synchronously across three Azure availability zones in the primary region.

- LRS provides a SLA 99.9999999999% (12 nines) over a year
- Recommended for scenarios that require HA
- Recommended for restricting replication of data to within a country or region to meet data governance requirements.

**Redundancy in the secondary region:**

Azure Storage offers two options for copying your data to a secondary region:

<strong>Geo-redundant Storage (GRS):</strong> copies your data synchronously three times within a single physical location in the primary region using LRS. It then copies your data asynchronously to a single physical location in the secondary region. Within the secondary region, your data is copied synchronously three times using LRS.

- LRS provides a SLA 99.99999999999999% (16 nines) over a year
- Recommended for scenarios that require HA

<strong>Geo-zone-redundant Storage (GZRS):</strong> copies your data synchronously across three Azure availability zones in the primary region using ZRS. It then copies your data asynchronously to a single physical location in the secondary region. Within the secondary region, your data is copied synchronously three times using LRS.

- LRS provides a SLA 99.99999999999999% (16 nines) over a year
- Recommended for scenarios that require HA
- Data is also usable during a complete regional outage or a disaster

# Durability and Availability Parameters

<p align=center>
<img src="..../assets/storagereplication1.png" alt="Storage Replication" title="Storage Replication"> </p>

# Durability and Availability by Outage Scenario

<p align=center>
<img src="..../assets/storagereplication2.png" alt="Outage Scenario" title="Outage Scenario"> </p>