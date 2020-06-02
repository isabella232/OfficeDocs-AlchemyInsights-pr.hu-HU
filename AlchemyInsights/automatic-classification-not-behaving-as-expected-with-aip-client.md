---
title: Az automatikus besorolás nem a várt módon viselkedik az AIP-ügyféllel
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
- "4373"
ms.openlocfilehash: 22eeb6ba32e4e943efa2495a477ff394f3c135db
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508378"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Az automatikus besorolás nem a várt módon viselkedik az AIP-ügyféllel

Az automatikus besorolás nem a várt módon viselkedik, kövesse az alábbi ajánlott irányelveket:

1. Ha problémái vannak az automatikus címkézéssel, olvassa [el A feltételek konfigurálása az Azure Information Protection automatikus és ajánlott besorolásához,](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) és [hogy milyen bizalmas információtípusokat keresnek.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
2. Ellenőrizze, hogy olyan hatókörrel kapcsolatos szabályzatokat használ-e, amelyek nincsenek megfelelően konfigurálva: [Az Azure Information Protection szabályzat konfigurálása adott felhasználók számára hatókörrel kapcsolatos szabályzatok használatával.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)
3. Ha az automatikus címkézés nem működik az Outlook programban, amikor címkézett dokumentumot csatol, ellenőrizze, hogy `DRMEncryptProperty` nincs-e definiálva az itt leírtak szerint: [Tartalomvédelmi szolgáltatás beállításjegyzék-beállításai biztonsági okokból.](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)
4. Ha az Azure Information Protection szabályzathoz a [beépített adattípusokat](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) használta, ellenőrizze, hogy a tartalom megfelel-e a várt formátumnak.
5. Ellenőrizze, hogy a címke megfelelően van-e konfigurálva az **Automatikus** vagy **az Ajánlott**felirathoz. (**Az automatikus** címkézés minden Office-alkalmazásban elérhető, míg az **Ajánlott** az Outlook kivételével minden Office-alkalmazáshoz elérhető.)
6. Nem használhatja az automatikus besorolást olyan dokumentumokhoz és e-mailekhez, amelyeket korábban manuálisan címkéztek vagy korábban automatikusan magasabb besorolással címkéztek.  További információ: [Az automatikus vagy ajánlott címkék alkalmazása.](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied)
7. Ha továbbra is problémákat tapasztal, gyűjtse össze az Azure Information Protection ügyfélnaplókat, és csatolja az exportált naplókat a támogatási jegyhez. Az Azure Information Protection naplóinak exportálása:
    - Nyisson meg egy Office-dokumentumot, vagy hozzon létre egy új e-mailt az Outlookban.
    - Kattintson **a Védelem/érzékenység**  >  **súgó és visszajelzés gombra.**
    - Kattintson **a Naplók exportálása gombra.**
    - Mentse a naplókat a választott helyre, és csatolja őket a szolgáltatási kérelemhez.

További információ:

- [Az Azure Information Protection automatikus és ajánlott besorolási feltételeinek konfigurálása](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Útmutató útmutatók az Azure Information Protectiont használó gyakori forgatókönyvekhez](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Tekintse át az Azure Information Protection dokumentációját](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Tekintse át az Azure Information Protection előfizetéseit és funkcióit](https://azure.microsoft.com/pricing/details/information-protection)
- [Az Azure-információvédelem követelményei](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Rövid útmutató az Azure Information Protection szolgáltatáshoz](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Az Azure Information Protection ügyfél letöltése](https://www.microsoft.com/download/details.aspx?id=53018)
