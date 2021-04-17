---
title: Egy Microsoft 365-csoport e-mail-címének módosítása
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 8eaafae8650a8072cdfbec281afe6d5e93fea655
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819046"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="c399a-102">Egy Microsoft 365-csoport e-mail-címének módosítása</span><span class="sxs-lookup"><span data-stu-id="c399a-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="c399a-103">A felügyeleti központban módosíthatja egy Microsoft 365-csoport e-mail-címét.</span><span class="sxs-lookup"><span data-stu-id="c399a-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="c399a-104">Egyszerűen jelölje ki a csoportot, majd válassza az @E-mail-cím szerkesztése lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="c399a-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="c399a-105">A következő EXO PowerShell-parancsot is használhatja egy Microsoft 365-csoport elsődleges SMTP-címének megváltoztatásához:</span><span class="sxs-lookup"><span data-stu-id="c399a-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="c399a-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="c399a-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="c399a-107">Példa:</span><span class="sxs-lookup"><span data-stu-id="c399a-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
