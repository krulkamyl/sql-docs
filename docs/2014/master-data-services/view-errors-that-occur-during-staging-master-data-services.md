---
title: "View Errors that Occur During the Staging Process (Master Data Services) | Microsoft Docs"
ms.custom: ""
ms.date: "03/06/2017"
ms.prod: "sql-server-2014"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "master-data-services"
ms.tgt_pltfrm: ""
ms.topic: conceptual
helpviewer_keywords: 
  - "staging process [Master Data Services], viewing errors"
ms.assetid: 6d2bff84-624b-47fc-a4a5-d9ea01d13412
caps.latest.revision: 7
author: leolimsft
ms.author: lle
manager: craigg
---
# View Errors that Occur During the Staging Process (Master Data Services)
  In [!INCLUDE[ssMDSshort](../includes/ssmdsshort-md.md)], you can view errors that occur during the staging process. In the [!INCLUDE[ssMDSshort](../includes/ssmdsshort-md.md)] database, there are two views that show errors:  
  
-   stg.viw_name_MemberErrorDetails for leaf or consolidated member updates.  
  
-   stg.viw_name_RelationshipErrorDetails for hierarchy relationship updates.  
  
## Prerequisites  
 To perform this procedure:  
  
-   In the [!INCLUDE[ssMDSshort](../includes/ssmdsshort-md.md)] database, you must have SELECT permissions to either the stg.viw_name_MemberErrorDetails or stg.viw_name_RelationshipErrorDetails view.  
  
-   You must be a model administrator. For more information, see [Administrators &#40;Master Data Services&#41;](administrators-master-data-services.md).  
  
### To view staging errors  
  
1.  Open [!INCLUDE[ssManStudioFull](../includes/ssmanstudiofull-md.md)] and connect to the [!INCLUDE[ssDE](../includes/ssde-md.md)] instance for your [!INCLUDE[ssMDSshort](../includes/ssmdsshort-md.md)] database.  
  
2.  Open a new query.  
  
3.  Type the following text, replacing name with the name of your staging table, for example, viw_Product_MemberErrorDetails.  
  
     `SELECT * FROM stg.viw_name_MemberErrorDetails`  
  
4.  Excecute the query. Error details are displayed in the **ErrorDescription** field.  
  
## Next Steps  
 For more details on error messages, see [Staging Process Errors &#40;Master Data Services&#41;](../../2014/master-data-services/staging-process-errors-master-data-services.md).  
  
## See Also  
 [Data Import &#40;Master Data Services&#41;](overview-importing-data-from-tables-master-data-services.md)   
 [Troubleshooting the Staging Process (Master Data Services)](http://social.technet.microsoft.com/wiki/contents/articles/troubleshooting-the-staging-process-master-data-services.aspx)  
  
  