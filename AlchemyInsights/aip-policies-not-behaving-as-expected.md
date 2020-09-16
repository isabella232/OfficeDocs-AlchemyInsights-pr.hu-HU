---
title: 'Rendszergazda: a házirendek nem a várt módon viselkednek.'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663191"
---
# <a name="aip-policies-not-behaving-as-expected"></a>Rendszergazda: a házirendek nem a várt módon viselkednek.

Azure Information Protection: a házirendek a várttól eltérő módon működnek

1. Ha a vizuális jelzésekkel kapcsolatos problémákat tapasztal, olvassa el a [vizuális jelzések alkalmazása](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)esetén című témakört.
2. Ha problémák merülnek fel az automatikus címkézés során, kérjük, tekintse át, hogyan konfigurálhatja az Azure-alapú adatvédelem és [a bizalmas adattípusok](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) [automatikus és ajánlott besorolási feltételeit](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) .
3. Ha a natív/Pfile védelem során problémákat tapasztal, olvassa el a [fájlok API-konfigurációjának](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)áttekintése című témakört.
4. Ellenőrizze, hogy léteznek-e olyan hatókörű házirendek, amelyek nincs megfelelően konfigurálva: [Az Azure-adatvédelem házirendjének konfigurálása meghatározott felhasználókhoz hatóköres házirendek használatával](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Ha a címkével ellátott dokumentumok csatolásakor az automatikus címkézés nem mûködik az Outlookban, ellenőrizze, hogy a DRMEncryptProperty nem az itt ismertetett módon van definiálva: [a tartalomvédelmi szolgáltatás beállításjegyzékének beállításai](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Ha továbbra is problémákat tapasztal, kérjük, gyűjtsön az Azure Information Protection ügyfél naplóit, és csatolja az exportált naplókat a jegyhez.

1. Nyisson meg egy Office-dokumentumot, vagy hozzon létre egy új e-mailt az Outlookban.
2. Kattintson a **védelem/érzékenység**  >  **Súgó és visszajelzés**elemre.
3. Kattintson a **naplók exportálása**parancsra.
4. Mentse a naplókat a kívánt helyre, és csatolja őket a szolgáltatási kéréshez.

További források:

- [Címke beállítása az Azure-védelemhez használható vizuális jelzésekhez](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Az Azure Information Protection dokumentációjának áttekintése](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Tartalmi címkék használata a Microsoft 365-alkalmazásokban](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

