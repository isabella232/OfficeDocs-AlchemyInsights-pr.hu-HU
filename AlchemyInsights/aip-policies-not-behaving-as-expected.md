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
ms.openlocfilehash: 90448bf57297ce59ba222efd1927b5de588bfbfdb1206b6403764d7f43fed690
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934295"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: A házirendek nem a várt módon viselkednek

Azure Information Protection: A házirendek nem a várt módon viselkednek. A különböző házirendekkel kapcsolatos problémákhoz az alábbi ajánlott irányelveket ajánljuk:

1. Ha problémákat jelentkezik a vizuális jelölésekkel kapcsolatban, kérjük, olvassa el a Vizuális [jelölések alkalmazásakor.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)
2. Ha problémákat okozhat az automatikus címkézéssel kapcsolatban, olvassa el a Feltételek konfigurálása az [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) automatikus és ajánlott besorolásához és A bizalmas [adattípusok által keresnek.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
3. Ha natív/Pfile protection-problémákat jelentkezik, tekintse át a [Fájl API-konfigurációt.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)
4. Ellenőrizze, hogy nem használ-e nem megfelelően konfigurált, hatókörrel rendelkező házirendeket: [Az Azure Information Protection házirend konfigurálása adott felhasználók számára a hatókörrel rendelkező házirendek használatával](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Ha az automatikus feliratozás nem működik az Outlook-hoz címkeként megadott dokumentum csatolása esetén, ellenőrizze, hogy a DRMEncryptProperty nincs-e definiálva a következő módon: A biztonság IRM beállításjegyzékének [beállításai.](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)

Ha továbbra is problémákat tapasztal, gyűjtse össze az Azure Information Protection-ügyfélnaplókat, és csatolja az exportált naplókat ehhez a jegyhez.

1. Nyisson meg egy Office-dokumentumot, vagy hozzon létre egy új e-mailt az Outlookban.
2. Kattintson a **Védelem/Érzékenység** > **Súgó és visszajelzés** elemre.
3. Kattintson a **Naplók exportálása** gombra.
4. Mentse a naplókat a választott helyre, és csatolja őket ehhez a szolgáltatáskéréshez.

További források:

- [Címke beállítása vizuális jelöléshez az Azure Information Protectionben](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Az Azure Information Protection dokumentációjának áttekintése](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Bizalmasság-címkék használata Microsoft 365 alkalmazásokban](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

