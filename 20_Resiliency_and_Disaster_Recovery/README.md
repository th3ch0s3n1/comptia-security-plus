# 🔄 Section 20: Resiliency & Disaster Recovery


> Cornell Notes — CompTIA Security+ (SY0-701) | Maps to Domain 3.0 & Domain 5.0 (Security Architecture / Security Program Management and Oversight)


## ❓ Cue / Key Questions & Notes


| Question / Keyword | Answer |
| --- | --- |
| **🟢 Architecture Resiliency** |  |
| 🔴 What is resiliency? | The structural capacity of an architecture to maintain acceptable operational service levels despite active faults, structural failures, or malicious disruptions. |
| 🔴 What is high availability? | HA; system design implementations that ensure operational continuity and minimize downtime over a prolonged measurement window. |
| **🟢 Storage Redundancy** | RAID |
| 🔴 What is RAID? | Redundant Array of Independent Disks; grouping multiple physical hard drives together into a single logical volume to achieve performance gains, fault tolerance, or both. |
| 🔴 RAID 0 vs. RAID 1 | RAID 0 uses **striping** for raw data access speed but offers zero fault tolerance; RAID 1 uses **mirroring** to write identical data to two disks simultaneously for immediate failover protection. |
| 🔴 What is RAID 5? | Striping with distributed parity; allows the array to survive the total loss of a single disk. Requires a minimum of 3 drives. |
| 🔴 What is RAID 6? | Striping with dual distributed parity; allows the array to survive the simultaneous loss of 2 disks. Requires a minimum of 4 drives. |
| 🔴 What is RAID 10? | A stripe of mirrors (RAID 1+0); combines the high write performance of striping with the redundancy of mirroring. Requires a minimum of 4 drives. |
| **🟢 Backup Operations** |  |
| 🔴 What is a full backup? | Captures all selected system data in a single operation and clears the archive bits. It serves as the baseline for all other backup types. |
| 🔴 What is a differential backup? | Copies all data files modified *since the last full backup*. It does not clear archive bits, meaning file size grows sequentially until the next full backup. |
| 🔴 What is an incremental backup? | Copies only the files modified *since the last backup of any kind*. It clears the archive bits, resulting in rapid backup times but longer restoration paths. |
| 🔴 What is a system snapshot? | A lightweight point-in-time virtual state capture of a virtual machine or volume, allowing fast rollbacks to a known-good configuration. |
| 🔴 What is the 3-2-1 backup rule? | Maintain **3** total copies of data, stored across **2** different types of physical media, with at least **1** copy kept completely offsite. |
| **🟢 Disaster Recovery Sites** |  |
| 🔴 What is a hot site? | A fully operational, identical duplicate facility with active hardware, communication links, and real-time data replication, allowing near-instantaneous failover. |
| 🔴 What is a warm site? | A secondary facility equipped with required hardware and network connections, but lacking live data synchronization. It requires restoring backups before becoming operational. |
| 🔴 What is a cold site? | An empty operational shell providing physical space, power, and environmental cooling, but requiring complete hardware transport and setup to function. |
| 🔴 What is geographic dispersal? | Strategically locating redundant data facilities across distinct geographic regions to ensure a single localized catastrophe (e.g., an earthquake) cannot destroy both environments. |
| **🟢 Infrastructure Infrastructure** | UPS |
| 🔴 UPS vs. Generator | An Uninterruptible Power Supply (UPS) provides near-instantaneous battery power to prevent data corruption during initial power drops; backup generators handle long-term power generation during extended utility blackouts. |
| 🔴 What are dual power supplies? | Equipping critical hardware with two independent internal power units routed into separate electrical circuits to eliminate a single point of failure. |


## 📝 Summary


Organizational continuity relies on **architecture resiliency** and engineered redundancy across every level of the infrastructure. At the data layer, system availability is maintained via **RAID configurations**—balancing the speed of RAID 0 striping against the fault tolerance of RAID 1 mirroring, or deploying parity arrays like RAID 5, RAID 6, and hybrid RAID 10 setups. These storage environments are defended using regular data retention routines matching the **3-2-1 backup rule**, combining standalone **full backups** with rapid **incremental** processes, cumulative **differential** captures, or virtual system **snapshots**. When addressing catastrophic site-wide infrastructure drops, enterprise disaster recovery plans rely on **geographic dispersal** across tier-structured backup environments, scaling from bare physical **cold sites** and partially equipped **warm sites** up to mirror-synchronized **hot sites**. Finally, on-premise components protect against minor infrastructure failures through automated technical primitives, combining localized battery **UPS** systems and secondary **generators** with **dual power supplies** to eliminate single points of failure.
