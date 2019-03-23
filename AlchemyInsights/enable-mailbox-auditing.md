---
title: Postaláda naplózásának engedélyezése
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 81041685cf383a231a9a9739d6daffd6039b4602
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/22/2019
ms.locfileid: "30757820"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="25f5b-102">Postaláda naplózásának engedélyezése</span><span class="sxs-lookup"><span data-stu-id="25f5b-102">Enable mailbox auditing</span></span>

<span data-ttu-id="25f5b-103">Postaláda naplózásának engedélyezése egy felhasználó vagy a teljes szervezet számára a következő parancsmagok távoli energiagazdálkodási rendszerhéj kell futtatni:</span><span class="sxs-lookup"><span data-stu-id="25f5b-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="25f5b-104">**Egyfelhasználós**</span><span class="sxs-lookup"><span data-stu-id="25f5b-104">**Single User**</span></span>
  
<span data-ttu-id="25f5b-105">Set-Mailbox - identitás "Judit Dow" - AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="25f5b-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="25f5b-106">**Szervezet**</span><span class="sxs-lookup"><span data-stu-id="25f5b-106">**Organization**</span></span>
  
<span data-ttu-id="25f5b-107">Get-postaláda - ResultSize korlátlan - szűrése a {RecipientTypeDetails - eq "UserMailbox"} |}] Set-Mailbox - AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="25f5b-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="25f5b-108">tudj meg többet</span><span class="sxs-lookup"><span data-stu-id="25f5b-108">Learn more</span></span>](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

