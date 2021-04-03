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
ms.openlocfilehash: 6f640093cd099f20d3a95eede5c141ad74838b0b
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505688"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="cee78-102">Törölt Microsoft 365-csoport visszaállítása</span><span class="sxs-lookup"><span data-stu-id="cee78-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="cee78-103">A törölt Microsoft 365-csoportokat és Microsoft Teamseket a törléstől számított 30 napon belül visszaállíthatja.</span><span class="sxs-lookup"><span data-stu-id="cee78-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="cee78-104">Ha be kell jelentkeznie a Microsoft 365 Felügyeleti központba, és fel kell sorolni a törölt csoportokat és csoportokat, lépjen a [Microsoft 365 Felügyeleti központba.](https://aka.ms/RestoreDeletedGroup)</span><span class="sxs-lookup"><span data-stu-id="cee78-104">To login to Microsoft 365 admin center and list the deleted groups and teams, go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup).</span></span>

    <span data-ttu-id="cee78-105">**Megjegyzés:** Jelentkezzen be a bérlői rendszergazdai vagy a csoport-rendszergazdai szerepkörhöz hozzárendelt fiókkal.</span><span class="sxs-lookup"><span data-stu-id="cee78-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="cee78-106">Jelölje ki a visszaállítani kívánt törölt Microsoft 365-csoportot/Teamst, és kattintson a **csoport visszaállítása elemre.**</span><span class="sxs-lookup"><span data-stu-id="cee78-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="cee78-107">Ha a csoport nem állítható vissza ütköző SMTP-cím miatt, az alábbi paranccsal keresse meg az ütközést okozó objektumot, és távolítsa el az SMTP-címet:</span><span class="sxs-lookup"><span data-stu-id="cee78-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="cee78-108">**Megjegyzés:** Bizonyos esetekben akár 24 óra is elehet, amíg a csoport és az összes adata visszaállítható.</span><span class="sxs-lookup"><span data-stu-id="cee78-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="cee78-109">További információért, illetve a csoportok PowerShell használatával való visszaállításáról a Törölt [Microsoft 365-csoport](https://go.microsoft.com/fwlink/?linkid=867802)visszaállítása.</span><span class="sxs-lookup"><span data-stu-id="cee78-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>