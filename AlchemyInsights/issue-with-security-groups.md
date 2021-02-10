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
# <a name="issue-with-security-groups"></a>Biztonsági csoportokkal kapcsolatos probléma

**Ha hálózati hibát kap az AADDS104-ben**

Az Azure Active Directory tartományi szolgáltatások (AD DS) hálózati hibáinak leggyakoribb oka az érvénytelen hálózati biztonsági csoport szabályai. A virtuális hálózat hálózati biztonsági csoportjának engedélyeznie kell bizonyos portokhoz és protokollokhoz való hozzáférést. Ha ezek a portok le vannak tiltva, az Azure platform nem tudja figyelni vagy frissíteni a felügyelt tartományt. Az Azure AD és az Azure AD DS közötti szinkronizálás is érintett. Győződjön meg arról, hogy az alapértelmezett portok nyitva maradnak, hogy elkerülje a szolgáltatáskimaradást.

A hálózati biztonsági csoportok konfigurációs problémáival kapcsolatos gyakori riasztásokért és azok elhárításáról a Biztonsági csoportok hozzáadása és [ellenőrzése cikkből értesül.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules)
