---
description: "sys.dm_xe_session_event_actions (Transact-SQL)"
title: "sys.dm_xe_session_event_actions (Transact-SQL) | Microsoft Docs"
ms.custom: ""
ms.date: "06/10/2016"
ms.prod: sql
ms.reviewer: ""
ms.technology: system-objects
ms.topic: "reference"
f1_keywords: 
  - "dm_xe_session_event_actions_TSQL"
  - "sys.dm_xe_session_event_actions_TSQL"
  - "dm_xe_session_event_actions"
  - "sys.dm_xe_session_event_actions"
dev_langs: 
  - "TSQL"
helpviewer_keywords: 
  - "extended events [SQL Server], views"
  - "sys.dm_xe_session_event_actions dynamic management view"
ms.assetid: 0c22a546-683e-4c84-ab97-1e9e95304b03
author: rwestMSFT
ms.author: randolphwest
---
# sys.dm_xe_session_event_actions (Transact-SQL)
[!INCLUDE [SQL Server](../../includes/applies-to-version/sqlserver.md)]

  Returns information about event session actions. Actions are executed when events are fired.  
  
|Column name|Data type|Description|  
|-----------------|---------------|-----------------|  
|event_session_address|**varbinary(8)**|The memory address of the event session. Is not nullable.|  
|action_name|**nvarchar(256)**|The name of the action. Is not nullable.|  
|action_package_guid|**uniqueidentifier**|The GUID for the package that contains the action. Is not nullable.|  
|event_name|**nvarchar(256)**|The name of the event that the action is bound to. Is not nullable.|  
|event_package_guid|**uniqueidentifier**|The GUID for the package that contains the event. Is not nullable.|  
  
## Permissions  
 Requires VIEW SERVER STATE permission on the server.  
  
### Relationship Cardinalities  
  
|From|To|Relationship|  
|----------|--------|------------------|  
|sys.dm_xe_session_event_actions.event_session_address|sys.dm_xe_sessions.address|Many-to-one|  
|sys.dm_xe_session_event_actions.action_name,<br /><br /> sys.dm_xe_session_event_actions.action_package_guid|sys.dm_xe_objects.name,<br /><br /> sys.dm_xe_session_events.event_package_guid|Many-to-one|  
|sys.dm_xe_session_event_actions.event_name,<br /><br /> sys.dm_xe_session_event_actions.event_package_guid|sys.dm_xe_objects.name,<br /><br /> sys.dm_xe_objects.package_guid|Many-to-one|  
  
## See Also  
 [Dynamic Management Views and Functions &#40;Transact-SQL&#41;](~/relational-databases/system-dynamic-management-views/system-dynamic-management-views.md)  
  
  

