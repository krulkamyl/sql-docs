---
description: "ISJSON (Transact-SQL)"
title: "ISJSON (Transact-SQL) | Microsoft Docs"
ms.custom: ""
ms.date: 06/03/2020
ms.prod: sql
ms.technology: t-sql
ms.topic: reference
f1_keywords: 
  - "ISJSON"
  - "ISJSON_TSQL"
helpviewer_keywords: 
  - "ISJSON function"
  - "JSON, validating"
ms.assetid: c836f3d3-3e17-44ae-92bf-f341918896c3
author: "jovanpop-msft"
ms.author: "jovanpop"
monikerRange: "= azuresqldb-current||= azure-sqldw-latest||>= sql-server-2016||>= sql-server-linux-2017"
---
# ISJSON (Transact-SQL)
[!INCLUDE [sqlserver2016-asdb-asdbmi-asa](../../includes/applies-to-version/sqlserver2016-asdb-asdbmi-asa.md)]

  Tests whether a string contains valid JSON.  
  
 ![Topic link icon](../../database-engine/configure-windows/media/topic-link.gif "Topic link icon") [Transact-SQL Syntax Conventions](../../t-sql/language-elements/transact-sql-syntax-conventions-transact-sql.md)  
  
## Syntax  
  
```syntaxsql  
ISJSON ( expression )  
```  
  
## Arguments
 *expression*  
 The string to test.  
  
## Return Value  
 Returns 1 if the string contains valid JSON; otherwise, returns 0. Returns null if *expression* is null.  
  
 Does not return errors.  
  
## Remarks  
 **ISJSON** does not check the uniqueness of keys at the same level.  
  
## Examples  
  
### Example 1  
The following example runs a statement block conditionally if the parameter value `@param` contains valid JSON.  
  
```sql  
DECLARE @param <data type>
SET @param = <value>

IF (ISJSON(@param) > 0)  
BEGIN  
     -- Do something with the valid JSON value of @param.  
END
```  
  
### Example 2  
The following example returns rows in which the column `json_col` contains valid JSON.  
  
```sql  
SELECT id, json_col
FROM tab1
WHERE ISJSON(json_col) > 0 
```  
  
## See Also  
 [JSON Data &#40;SQL Server&#41;](../../relational-databases/json/json-data-sql-server.md)  
  
  
