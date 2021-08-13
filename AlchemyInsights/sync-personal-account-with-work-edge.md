---
title: Személyes fiók szinkronizálásának engedélyezése egy felhasználónak a munkahelyi fiókkal a Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9127"
- "9004429"
ms.openlocfilehash: da435b37b689e97ca51ce5cf94eb7e7d71eb972060526989239310fac1460628
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813397"
---
# <a name="enable-a-user-to-sync-a-personal-account-with-the-work-account-in-microsoft-edge"></a>Személyes fiók szinkronizálásának engedélyezése egy felhasználónak a munkahelyi fiókkal a Microsoft Edge

Győződjön meg arról, hogy megfelel a következő feltételeknek:

- A nagyvállalati állapotroaming a Azure Active Directory Felügyeleti központban engedélyezett, amelyhez előfizetés szükséges a prémium szintű Azure Active Directory-Enterprise Mobility + Security(EMS). További információ: Vállalati központi roaming engedélyezése [Azure Active Directory.](/azure/active-directory/devices/enterprise-state-roaming-enable)
- Az alábbi feltételek egyike vagy mindkettő teljesül:
    - Az Azure Information Protection szolgáltatás engedélyezve van a bérlőjéhez. Részletekért lásd: A Azure Tartalomvédelmi szolgáltatások elleni védelem [aktiválása Microsoft 365 Felügyeleti központ.](/azure/information-protection/activate-office365)
    - Az Azure Active Directory vállalati központi roaming (ESR) szolgáltatás minden felhasználónál vagy bérlői fiókban engedélyezve van. További információt a Mi a nagyvállalati [államroaming? ?.](/azure/active-directory/devices/enterprise-state-roaming-overview)

Ha az AIP és a ESR is le van tiltva, hibaüzenet tájékoztatja a felhasználókat arról, hogy a fiókjukban nem érhető el a szinkronizálás.
