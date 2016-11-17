---
title: Delete an AppLocker Rule
description: "Windows Server Security"
ms.custom: na
ms.prod: windows-server-threshold
ms.reviewer: na
ms.suite: na
ms.technology: security-applocker
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: fdbff40d-394e-496b-8f24-08d7052b6762
author: coreyp-at-msft
ms.author: coreyp
manager: dongill
ms.date: 10/12/2016
---
# Delete an AppLocker Rule

>Applies To: Windows Server 2016, Windows Server 2012 R2, Windows Server 2012
This topic describes the steps to delete an AppLocker rule, which will prevent the application that is specified in the rule from running in Windows Server 2012 and Windows 8.

As older applications are retired and new applications are deployed in your organization, it will be necessary to modify the application control policies. If an application becomes unsupported by the IT department or is no longer allowed due to the organization's security policy, then deleting the rule or rules associated with that application will prevent the application from running.

For information about testing an AppLocker policy to see what rules affect which files or applications, see [Test an AppLocker Policy by Using Test-applockerPolicy](../policies/test-an-applocker-policy-by-using-test-applockerpolicy.md).

You can perform this task by using the Group Policy Management Console for an AppLocker policy in a Group Policy Object (GPO) or by using the Local Security Policy snap-in for an AppLocker policy on a local computer or in a security template. For information how to use these MMC snap-ins to administer AppLocker, see [Using the MMC snap-ins to administer AppLocker](../administer-applocker.md#BKMK_Using_Snapins).

### <a name="BKMK_DeleteAppLockerRuleGPO"></a>To delete a rule in an AppLocker policy

1.  In the console tree of the snap-in, double-click **Application Control Policies**, and then double-click **AppLocker**.

2.  Click the appropriate rule collection for which you want to delete the rule.

3.  In the details pane, right-click the rule to delete, click **Delete**, and then click **Yes**.

> [!NOTE]
> When using Group Policy, for the rule deletion to take effect on computers within the domain, the GPO must be distributed or refreshed.
> 
> When this procedure is performed on the local computer, the AppLocker policy takes effect immediately.

