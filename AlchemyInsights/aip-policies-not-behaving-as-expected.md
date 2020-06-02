---
title: 'AIP: A házirendek nem a várt módon viselkednek'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 7926ff9ebbd54969fb5b3ae5d909baffe96a4292
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/26/2020
ms.locfileid: "44493158"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: A házirendek nem a várt módon viselkednek

Azure Information Protection: Szabályzatok nem viselkednek a várt módon, lásd a következő ajánlott irányelvek különböző szabályzati problémák:

1. Ha vizuális jelölésekkel kapcsolatos problémái vannak, kérjük, olvassa el [A vizuális jelölések alkalmazásakor való áttekintést.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)
2. Ha problémái vannak az automatikus címkézéssel, tekintse át a [Hogyan konfigurálhatja az Azure Information Protection automatikus és ajánlott besorolási feltételeit,](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) és [hogy milyen bizalmas információtípusokat keresnek.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
3. Ha problémákat okoz a Ninatív/Pfile-védelemmel, tekintse át [a Fájl API-konfigurációját.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)
4. Ellenőrizze, hogy olyan hatókörrel kapcsolatos szabályzatokat használ-e, amelyek nincsenek megfelelően konfigurálva: [Az Azure Information Protection szabályzat konfigurálása adott felhasználók számára hatókörrel kapcsolatos szabályzatok használatával.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)
5. Ha az automatikus címkézés nem működik az Outlook programban, amikor címkézett dokumentumot csatol, ellenőrizze, hogy a DRMEncryptProperty nincs-e definiálva az itt leírtak szerint: [Tartalomvédelmi rendszerbiztonsági beállításjegyzék-beállítások](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Ha továbbra is problémákat tapasztal, gyűjtse össze az Azure Information Protection ügyfélnaplókat, és csatolja az exportált naplókat ehhez a jegyhez.

1. Nyisson meg egy Office-dokumentumot, vagy hozzon létre egy új e-mailt az Outlookban.
2. Kattintson **a Védelem/érzékenység**  >  **súgó és visszajelzés gombra.**
3. Kattintson **a Naplók exportálása gombra.**
4. Mentse a naplókat a választott helyre, és csatolja őket ehhez a szolgáltatási kérelemhez.

További források:

- [Az Azure Information Protection vizuális jelölései címkéjének konfigurálása](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Tekintse át az Azure Information Protection dokumentációját](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Érzékenységi címkék használata az Office-appokban](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

