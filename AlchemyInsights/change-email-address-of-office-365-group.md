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
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/27/2020
ms.locfileid: "44282925"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a><span data-ttu-id="7cfc4-102">Microsoft 365-csoport e-mail címének módosítása</span><span class="sxs-lookup"><span data-stu-id="7cfc4-102">Change email address of an Microsoft 365 group</span></span>

<span data-ttu-id="7cfc4-103">A Microsoft 365-csoportok e-mail címét a Felügyeleti központ segítségével módosíthatja.</span><span class="sxs-lookup"><span data-stu-id="7cfc4-103">You can change the email address of an Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="7cfc4-104">Csak válassza ki a csoportot, és válassza ki @edit e-mail címét.</span><span class="sxs-lookup"><span data-stu-id="7cfc4-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="7cfc4-105">Az EXO PowerShell parancs követésével módosíthatja egy Microsoft 365-csoport elsődleges SMTP-címét is:</span><span class="sxs-lookup"><span data-stu-id="7cfc4-105">You can also use following the EXO PowerShell command to change the primary SMTP address of an Microsoft 365 group:</span></span>

<span data-ttu-id="7cfc4-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="7cfc4-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="7cfc4-107">Példa:</span><span class="sxs-lookup"><span data-stu-id="7cfc4-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
