---
title: Unavailable Guilds & Connection Issues
date: 2018-04-13 15:54:00
resolved: true
resolvedWhen: 2018-04-13 17:30:00
# Possible severity levels: down, disrupted, notice
severity: down
affected:
  - API
section: issue
---

*Post-mortem*

At approximately 14:01, a Redis instance acting as the primary for a highly-available cluster used by our API services was migrated automatically by Google’s Cloud Platform. This migration caused the node to incorrectly drop offline, forcing the cluster to rebalance and trigger known issues with the way our API instances handle Redis failover. After resolving this partial outage, unnoticed issues on other services caused a cascading failure through Example Chat App’s real time system. These issues caused enough critical impact that Example Chat App’s engineering team was forced to fully restart the service, reconnecting millions of clients over a period of 20 minutes.


---

