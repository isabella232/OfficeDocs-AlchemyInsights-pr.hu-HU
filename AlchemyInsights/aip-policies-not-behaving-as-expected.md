---
title: 'AIP: A házirendek nem a várt módon viselkednek'
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
- "9002266"
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821629"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: A házirendek nem a várt módon viselkednek

Azure Information Protection: A házirendek nem a várt módon viselkednek. A különböző házirendekkel kapcsolatos problémákhoz az alábbi ajánlott irányelveket ajánljuk:

1. Ha problémákat jelentkezik a vizuális jelölésekkel kapcsolatban, kérjük, olvassa el a Vizuális [jelölések alkalmazásakor.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)
2. Ha problémákat okozhat az automatikus címkézéssel kapcsolatban, olvassa el a Feltételek konfigurálása az [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) automatikus és ajánlott besorolásához és A bizalmas [adattípusok által keresnek.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
3. Ha natív/Pfile protection-problémákat jelentkezik, tekintse át a [Fájl API-konfigurációt.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)
4. Ellenőrizze, hogy nem megfelelően konfigurált hatókörű házirendeket használ-e: Az Azure Information Protection házirend konfigurálása adott felhasználók számára hatókörű [házirendek használatával.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)
5. Ha az Outlookban nem működik az automatikus feliratozás, amikor címkével jelölt dokumentumot csatol, ellenőrizze, hogy a DRMEncryptProperty nincs-e definiálva a következő módon: [Biztonsági tartalomvédelmi beállításjegyzék-beállítások.](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)

Ha továbbra is problémákat tapasztal, gyűjtse össze az Azure Information Protection-ügyfélnaplókat, és csatolja az exportált naplókat ehhez a jegyhez.

1. Nyisson meg egy Office-dokumentumot, vagy hozzon létre egy új e-mailt az Outlookban.
2. Kattintson **a Védelem/bizalmasság – súgó** és visszajelzés  >  **elemre.**
3. Kattintson **a Naplók exportálása elemre.**
4. Mentse a naplókat a választott helyre, és csatolja őket ehhez a szolgáltatáskéréshez.

További források:

- [Címke beállítása vizuális jelöléshez az Azure Information Protectionben](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Az Azure Information Protection dokumentációjának áttekintése](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Bizalmasság-címkék használata a Microsoft 365-ös alkalmazásokban](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

