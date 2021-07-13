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
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/08/2021
ms.locfileid: "53381716"
---
# <a name="outbound-relay-pool"></a>Kimenő továbbítási készlet

A Microsoft módosítja az e-mailek továbbításának vagy továbbításának beállításait a Microsoft 365. Bizonyos esetekben az üzeneteket egy speciális továbbítókészletet használva továbbítja vagy továbbítja Microsoft 365 keresztül a továbbításon keresztül. A továbbítási készlet használatával küldött üzenetek a címzett levélszemétmappába kerülnek. További információ: [Kimenő kézbesítési készletek](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

A továbbítási készlet használatával kapcsolatos esetek elkerülése érdekében győződjön meg arról, hogy a továbbított/továbbított üzenetek megfelelnek az alábbi feltételek egyikének:

- A kimenő feladó a bérlő elfogadott tartománya.
- A feladó házirend-keretrendszere (SPF) az üzenet be- vagy Microsoft 365.
- A P2 feladó tartományában a domainKeys Identified Mail (DKIM) tartománynév jelenik meg, amikor az üzenet Microsoft 365.
 
A fenti feltételeknek megfelelő üzeneteket a rendszer nem továbbítja a továbbítási készleten keresztül.

Ha tartománya MX rekordja egy külső vagy helyszíni kiszolgálóra mutat, továbbfejlesztett szűrés használatával ellenőrizze, hogy helyes-e az SPF-ellenőrzés a bejövő e-maileknél, és hogy ne küldjön e-maileket a továbbítási készleten keresztül.

**Hogyan tudhatja meg, hogy hatással vannak-e a továbbítási készletre?**

Ha a továbbított vagy továbbított e-mailek a fenti feltételek valamelyikét használják, az üzenetek nem lesznek továbbítva a továbbítókészleten keresztül. Ha azonban egy üzenet továbbítási készleten keresztül történik, a kimenő kiszolgáló IP-címe a 40.95.0.0/16 tartományba esik, és a kimenő kiszolgáló neve **rly** értékeket tartalmaz a névben.

