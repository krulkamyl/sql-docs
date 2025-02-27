---
description: "JSON Functions (Transact-SQL)"
title: "JSON Functions (Transact-SQL) | Microsoft Docs"
ms.custom: ""
ms.date: 06/03/2020
ms.prod: sql
ms.technology: t-sql
ms.topic: reference
helpviewer_keywords: 
  - "JSON functions"
ms.assetid: ec97d451-06af-44a3-8304-305d410cfc8e
author: "jovanpop-msft"
ms.author: "jovanpop"
monikerRange: "= azuresqldb-current||= azure-sqldw-latest||>= sql-server-2016||>= sql-server-linux-2017"
---
# JSON Functions (Transact-SQL)

[!INCLUDE [sqlserver2016-asdb-asdbmi-asa](../../includes/applies-to-version/sqlserver2016-asdb-asdbmi-asa.md)]

Use the functions described on the pages in this section to validate or change JSON text or to extract simple or complex values.  
  
|Function|Description|  
|--------------|-----------------|  
|[ISJSON](../../t-sql/functions/isjson-transact-sql.md)|Tests whether a string contains valid JSON.|  
|[JSON_VALUE](../../t-sql/functions/json-value-transact-sql.md)|Extracts a scalar value from a JSON string.|  
|[JSON_QUERY](../../t-sql/functions/json-query-transact-sql.md)|Extracts an object or an array from a JSON string.|  
|[JSON_MODIFY](../../t-sql/functions/json-modify-transact-sql.md)|Updates the value of a property in a JSON string and returns the updated JSON string.|

 For more info about the built-in support for JSON in [!INCLUDE[ssNoVersion](../../includes/ssnoversion-md.md)], see [JSON Data &#40;SQL Server&#41;](../../relational-databases/json/json-data-sql-server.md).  

## See Also

 - [Validate, Query, and Change JSON Data with Built-in Functions &#40;SQL Server&#41;](../../relational-databases/json/validate-query-and-change-json-data-with-built-in-functions-sql-server.md)
 - [JSON Path Expressions &#40;SQL Server&#41;](../../relational-databases/json/json-path-expressions-sql-server.md)
 - [JSON Data &#40;SQL Server&#41;](../../relational-databases/json/json-data-sql-server.md)  
