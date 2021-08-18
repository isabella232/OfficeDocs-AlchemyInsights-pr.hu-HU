---
title: Kimenő továbbítási készlet
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: 7e5bb1fda1dec0c0f72d1944d54b6f2747a6e909
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326079"
---
# <a name="outbound-relay-pool"></a>Kimenő továbbítási készlet

A Microsoft módosítja az e-mailek továbbítása vagy továbbítása során a Microsoft 365. Bizonyos esetekben az üzenetek továbbítása vagy továbbítása Microsoft 365 továbbítva egy speciális továbbítókészlet használatával. A továbbítási készlet használatával küldött üzenetek a címzett levélszemétmappába kerülnek. További információ: [Kimenő kézbesítési készletek](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

A továbbítási készlet használatával kapcsolatos esetek elkerülése érdekében győződjön meg arról, hogy a továbbított/továbbított üzenetek megfelelnek az alábbi feltételek egyikének:

- A kimenő feladó a bérlő elfogadott tartománya.
- A feladói házirend keretrendszer (SPF) továbbítja az üzenetet, amikor Microsoft 365.
- Amikor az üzenet érkezik, a P2 feladó tartományán a domainKeys Identified Mail (DKIM) tartománynév jelenik Microsoft 365.
 
A fenti feltételeknek megfelelő üzeneteket a rendszer nem továbbítja a továbbítási készleten keresztül.

Ha tartománya MX rekordja egy külső vagy helyszíni kiszolgálóra mutat, továbbfejlesztett szűrés használatával ellenőrizze, hogy helyes-e az SPF-ellenőrzés a bejövő e-maileknél, és hogy ne küldjön e-maileket a továbbítási készleten keresztül.

**Hogyan tudhatja meg, hogy hatással vannak-e a továbbítási készletre?**

Ha a továbbított vagy továbbított e-mailek a fenti feltételek valamelyikét használják, az üzenetek nem lesznek továbbítva a továbbítókészleten keresztül. Ha azonban egy üzenet továbbítási készleten keresztül van elküldve, a kimenő kiszolgáló IP-címe a 40.95.0.0/16 tartományba esik, és a kimenő kiszolgáló neve **rly** értékeket tartalmaz a névben.

