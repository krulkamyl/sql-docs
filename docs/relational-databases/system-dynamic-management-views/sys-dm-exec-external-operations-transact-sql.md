---
description: "sys.dm_exec_external_operations (Transact-SQL)"
title: "sys.dm_exec_external_operations (Transact-SQL) | Microsoft Docs"
ms.custom: ""
ms.date: "03/15/2017"
ms.prod: sql
ms.prod_service: "database-engine, sql-database, synapse-analytics, pdw"
ms.reviewer: ""
ms.technology: system-objects
ms.topic: "reference"
f1_keywords: 
  - "DM_EXEC_EXTERNAL_OPERATIONS_TSQL"
  - "DM_EXEC_EXTERNAL_OPERATIONS"
  - "SYS.DM_EXEC_EXTERNAL_OPERATIONS_TSQL"
dev_langs: 
  - "TSQL"
helpviewer_keywords: 
  - "PolyBase,views"
  - "PolyBase"
  - "sys.dm_exec_external_operations management view"
  - "dm_exec_external_operations management view"
ms.assetid: d268217a-85b8-4b7f-9cd1-87865eba2be1
author: rwestMSFT
ms.author: randolphwest
monikerRange: ">=sql-server-2016||>=sql-server-linux-2017||=azuresqldb-mi-current"
---
# sys.dm_exec_external_operations (Transact-SQL)
[!INCLUDE [sqlserver2016](../../includes/applies-to-version/sqlserver2016.md)]

  Captures information about external PolyBase operations.  
  
|Column Name|Data Type|Description|Range|  
|-----------------|---------------|-----------------|-----------|  
|execution_id|**nvarchar(32)**|Unique query identifier associated with PolyBase query|See ID in [sys.dm_exec_requests &#40;Transact-SQL&#41;](../../relational-databases/system-dynamic-management-views/sys-dm-exec-requests-transact-sql.md)|  
|step_index|**int**|Index of the query step|See step_index in [sys.dm_exec_distributed_request_steps &#40;Transact-SQL&#41;](../../relational-databases/system-dynamic-management-views/sys-dm-exec-distributed-request-steps-transact-sql.md)|  
|operation_ type|**nvarchar(128)**|Describes a Hadoop operation or other external operation|'External Hadoop Operation'|  
|operation_ name|**nvarchar(4000)**|Indicates how the status of job in percentage (how much is the input consumed)|0-1 - multiplied by factor 100 (completed)|  
|map_  progress|**float**|Indicates how the status of a reduce job in percentage, if any|0-1 - multiplied by factor 100 (completed)|  
  
## See Also  
 [PolyBase troubleshooting with dynamic management views](/previous-versions/sql/sql-server-2016/mt146389(v=sql.130))   
 [Dynamic Management Views and Functions &#40;Transact-SQL&#41;](~/relational-databases/system-dynamic-management-views/system-dynamic-management-views.md)   
 [Database Related Dynamic Management Views &#40;Transact-SQL&#41;](../../relational-databases/system-dynamic-management-views/database-related-dynamic-management-views-transact-sql.md)  
  
