---
title: Egy Microsoft 365-csoport vagy a Microsoft Teams e-mail-címének módosítása
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
ms.openlocfilehash: 7800a447c5dfcc8397121e1149921916ff7944ac
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819082"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a><span data-ttu-id="8ca99-102">Egy Microsoft 365-csoport vagy a Microsoft Teams e-mail-címének módosítása</span><span class="sxs-lookup"><span data-stu-id="8ca99-102">Change email address of a Microsoft 365 group or Microsoft Teams</span></span>

<span data-ttu-id="8ca99-103">A [Microsoft 365 Felügyeleti központban](https://admin.microsoft.com/) módosíthatja egy Microsoft 365-csoport vagy a Microsoft Teams e-mail-címét.</span><span class="sxs-lookup"><span data-stu-id="8ca99-103">You can change the email address of a Microsoft 365 group or Microsoft Teams by using the [Microsoft 365 admin center](https://admin.microsoft.com/).</span></span> <span data-ttu-id="8ca99-104">Egyszerűen jelölje ki a csoportot, majd válassza az @E-mail-cím szerkesztése lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="8ca99-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="8ca99-105">A következő EXO PowerShell-parancsot is használhatja egy Microsoft 365-csoport, illetve a Teams elsődleges SMTP-címének megváltoztatásához:</span><span class="sxs-lookup"><span data-stu-id="8ca99-105">You can also use the following EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group/Teams:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="8ca99-106">Példa:</span><span class="sxs-lookup"><span data-stu-id="8ca99-106">Example:</span></span>

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
