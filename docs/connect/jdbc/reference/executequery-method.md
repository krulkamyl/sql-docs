---
description: "executeQuery Method ()"
title: "executeQuery Method () | Microsoft Docs"
ms.custom: ""
ms.date: "01/19/2017"
ms.prod: sql
ms.prod_service: connectivity
ms.reviewer: ""
ms.technology: connectivity
ms.topic: reference
apiname: 
  - "SQLServerPreparedStatement.executeQuery ()"
apilocation: 
  - "sqljdbc.jar"
apitype: "Assembly"
ms.assetid: 1d90407f-16df-4ba2-b4a5-47d5751e1d7c
author: David-Engel
ms.author: v-davidengel
---
# executeQuery Method ()
[!INCLUDE[Driver_JDBC_Download](../../../includes/driver_jdbc_download.md)]

  Runs the SQL query in this [SQLServerPreparedStatement](../../../connect/jdbc/reference/sqlserverpreparedstatement-class.md) object and returns the [SQLServerResultSet](../../../connect/jdbc/reference/sqlserverresultset-class.md) object that is generated by the query.  
  
## Syntax  
  
```  
  
public java.sql.ResultSet executeQuery()  
```  
  
## Return Value  
 A SQLServerResultSet object.  
  
## Exceptions  
 [SQLServerException](../../../connect/jdbc/reference/sqlserverexception-class.md)  
  
## Remarks  
 This executeQuery method is specified by the executeQuery method in the java.sql.PreparedStatement interface.  
  
## See Also  
 [executeQuery Method &#40;SQLServerPreparedStatement&#41;](../../../connect/jdbc/reference/executequery-method-sqlserverpreparedstatement.md)   
 [SQLServerPreparedStatement Members](../../../connect/jdbc/reference/sqlserverpreparedstatement-members.md)   
 [SQLServerPreparedStatement Class](../../../connect/jdbc/reference/sqlserverpreparedstatement-class.md)  
  
  
