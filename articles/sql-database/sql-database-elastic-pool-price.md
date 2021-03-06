---
title: SQL Database elastic pool price and performance
description: Pricing information specific to elastic pools.
services: sql-database
documentationcenter: ''
author: srinia
manager: jhubbard
editor: ''

ms.assetid: e8d64ce5-e30a-445d-8c18-35b3825c6e76
ms.service: sql-database
ms.custom: multiple databases
ms.devlang: NA
ms.date: 05/27/2016
ms.author: srinia
ms.workload: data-management
ms.topic: article
ms.tgt_pltfrm: NA

---
# elastic pool billing and pricing information
elastic pools are billed per the following characteristics:

* An elastic pool is billed upon its creation, even when there are no databases in the pool.
* An elastic pool is billed hourly. This is the same metering frequency as for performance levels of standalone databases.
* If an elastic pool is resized to a new amount of eDTUs, then the pool is not billed according to the new amount of eDTUS until the resizing operation completes. This follows the same pattern as changing the performance level of standalone databases.
* The price of an elastic pool is based on the number of eDTUs of the pool. The price of an elastic pool is independent of the number and utilization of the elastic databases within it.
* Price is computed by (number of pool eDTUs)x(unit price per eDTU).

The unit eDTU price for an elastic pool is higher than the unit DTU price for a standalone database in the same service tier. For details, see [SQL Database pricing](https://azure.microsoft.com/pricing/details/sql-database/). 

To understand the eDTUs and service tiers, see [SQL Database options and performance](sql-database-service-tiers.md).

## Next steps
* [Create an elastic pool](sql-database-elastic-pool-create-portal.md)
* [Monitor, manage, and size an elastic pool](sql-database-elastic-pool-manage-portal.md)
* [SQL Database options and performance: understand what's available in each service tier](sql-database-service-tiers.md)
* [PowerShell script for identifying databases suitable for an elastic pool](sql-database-elastic-pool-database-assessment-powershell.md)

