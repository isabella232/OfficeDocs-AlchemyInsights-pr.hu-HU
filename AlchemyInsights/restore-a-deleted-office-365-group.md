---
title: Törölt Microsoft 365-csoport visszaállítása
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: b72b7c93ce9fe1b90d1608811b0eeabc8aec1363
ms.sourcegitcommit: a5edaaefdc56f8d5c8220a335f4e8228e2de4ee0
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/08/2021
ms.locfileid: "51645133"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="ab3e7-102">Törölt Microsoft 365-csoport visszaállítása</span><span class="sxs-lookup"><span data-stu-id="ab3e7-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="ab3e7-103">A törölt Microsoft 365-csoportokat és Microsoft Teamseket a törléstől számított 30 napon belül visszaállíthatja.</span><span class="sxs-lookup"><span data-stu-id="ab3e7-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="ab3e7-104">Lépjen a [Microsoft 365](https://aka.ms/RestoreDeletedGroup) Felügyeleti központba, és jelentkezzen be a törölt csoportok és csapatok listájába.</span><span class="sxs-lookup"><span data-stu-id="ab3e7-104">Go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup) to log in to a list of your the deleted groups and teams.</span></span>

    <span data-ttu-id="ab3e7-105">**Megjegyzés:** Jelentkezzen be a bérlői rendszergazdai vagy a csoport-rendszergazdai szerepkörhöz hozzárendelt fiókkal.</span><span class="sxs-lookup"><span data-stu-id="ab3e7-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="ab3e7-106">Jelölje ki a visszaállítani kívánt törölt Microsoft 365-csoportot/Teamst, és kattintson a **csoport visszaállítása elemre.**</span><span class="sxs-lookup"><span data-stu-id="ab3e7-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="ab3e7-107">Ha a csoport nem állítható vissza ütköző SMTP-cím miatt, az alábbi paranccsal keresse meg az ütközést okozó objektumot, és távolítsa el az SMTP-címet:</span><span class="sxs-lookup"><span data-stu-id="ab3e7-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="ab3e7-108">**Megjegyzés:** Bizonyos esetekben akár 24 óra is elehet, amíg a csoport és az összes adata visszaállítható.</span><span class="sxs-lookup"><span data-stu-id="ab3e7-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="ab3e7-109">További információért, illetve a csoportok PowerShell használatával való visszaállításáról a Törölt [Microsoft 365-csoport](https://go.microsoft.com/fwlink/?linkid=867802)visszaállítása.</span><span class="sxs-lookup"><span data-stu-id="ab3e7-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>