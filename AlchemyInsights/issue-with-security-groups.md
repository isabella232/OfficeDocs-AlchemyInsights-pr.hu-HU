---
title: Biztonsági csoportokkal kapcsolatos probléma
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177496"
---
# <a name="issue-with-security-groups"></a><span data-ttu-id="e0060-102">Biztonsági csoportokkal kapcsolatos probléma</span><span class="sxs-lookup"><span data-stu-id="e0060-102">Issue with security groups</span></span>

<span data-ttu-id="e0060-103">**Ha hálózati hibát kap az AADDS104-ben**</span><span class="sxs-lookup"><span data-stu-id="e0060-103">**If you are getting Network Error AADDS104**</span></span>

<span data-ttu-id="e0060-104">Az Azure Active Directory tartományi szolgáltatások (AD DS) hálózati hibáinak leggyakoribb oka az érvénytelen hálózati biztonsági csoport szabályai.</span><span class="sxs-lookup"><span data-stu-id="e0060-104">Invalid network security group rules are the most common cause of network errors for Azure Active Directory Domain Services (AD DS).</span></span> <span data-ttu-id="e0060-105">A virtuális hálózat hálózati biztonsági csoportjának engedélyeznie kell bizonyos portokhoz és protokollokhoz való hozzáférést.</span><span class="sxs-lookup"><span data-stu-id="e0060-105">The network security group for the virtual network must allow access to specific ports and protocols.</span></span> <span data-ttu-id="e0060-106">Ha ezek a portok le vannak tiltva, az Azure platform nem tudja figyelni vagy frissíteni a felügyelt tartományt.</span><span class="sxs-lookup"><span data-stu-id="e0060-106">If these ports are blocked, the Azure platform can't monitor or update the managed domain.</span></span> <span data-ttu-id="e0060-107">Az Azure AD és az Azure AD DS közötti szinkronizálás is érintett.</span><span class="sxs-lookup"><span data-stu-id="e0060-107">The synchronization between the Azure AD and Azure AD DS is also impacted.</span></span> <span data-ttu-id="e0060-108">Győződjön meg arról, hogy az alapértelmezett portok nyitva maradnak, hogy elkerülje a szolgáltatáskimaradást.</span><span class="sxs-lookup"><span data-stu-id="e0060-108">Ensure you keep the default ports open to avoid interruption in service.</span></span>

<span data-ttu-id="e0060-109">A hálózati biztonsági csoportok konfigurációs problémáival kapcsolatos gyakori riasztásokért és azok elhárításáról a Biztonsági csoportok hozzáadása és [ellenőrzése cikkből értesül.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules)</span><span class="sxs-lookup"><span data-stu-id="e0060-109">To understand and to resolve common alerts for network security group configuration issues, see [Add and Verify Security Groups](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span></span>
