---
title: Microsoft 365-csoport e-mail címének módosítása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580659"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="d091a-102">Microsoft 365-csoport e-mail címének módosítása</span><span class="sxs-lookup"><span data-stu-id="d091a-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="d091a-103">A Microsoft 365-csoportok e-mail címét a Felügyeleti központ segítségével módosíthatja.</span><span class="sxs-lookup"><span data-stu-id="d091a-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="d091a-104">Csak válassza ki a csoportot, és válassza ki @edit e-mail címét.</span><span class="sxs-lookup"><span data-stu-id="d091a-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="d091a-105">Az EXO PowerShell parancs követésével módosíthatja egy Microsoft 365-csoport elsődleges SMTP-címét is:</span><span class="sxs-lookup"><span data-stu-id="d091a-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="d091a-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="d091a-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="d091a-107">Példa:</span><span class="sxs-lookup"><span data-stu-id="d091a-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
