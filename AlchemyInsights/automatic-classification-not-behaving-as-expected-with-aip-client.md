---
title: Az automatikus besorolás nem a várt módon viselkedik az AIP ügyféllel
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
- "4373"
ms.openlocfilehash: 93d15b8b65fd52a567ecbb6e1f84363bf2b38946c105896b0b5ef41e49d16ea9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53979711"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Az automatikus besorolás nem a várt módon viselkedik az AIP ügyféllel

Ha az automatikus besorolás nem a várt módon viselkedik, használja az alábbi ajánlott útmutatót:

1. Ha problémákat tapasztal az automatikus címkézéssel kapcsolatban, olvassa el [Az Azure Information Protection automatikus és ajánlott besorolási feltételeinek konfigurálása](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) és [A bizalmas adatok keresett típusai](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) című témakört.
2. Ellenőrizze, hogy nem használ-e nem megfelelően konfigurált, hatókörrel rendelkező házirendeket: [Az Azure Information Protection házirend konfigurálása adott felhasználók számára a hatókörrel rendelkező házirendek használatával](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Ha címkézett dokumentum csatolása esetén az automatikus címkézés nem működik az Outlookban, győződjön meg arról, hogy a(z) `DRMEncryptProperty` nem az alábbi módon van definiálva: [IRM-beállításjegyzék biztonsági beállításai](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Ha az Azure Information Protection házirendhez [beépített információtípusokat](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) használt, ellenőrizze, hogy a tartalom megfelel az elvárt formátumnak.
5. Ellenőrizze, hogy a felirat megfelelően van-e konfigurálva az **Automatikus** vagy **Ajánlott** beállításhoz. (Az **Automatikus** címkézés az összes Microsoft 365-alkalmazáshoz elérhető, míg az **Ajánlott** az Outlook kivételével minden Microsoft 365-alkalmazáshoz elérhető.)
6. Nem használhat automatikus besorolást olyan dokumentumokhoz és e-mailekhez, amelyeket korábban manuálisan címkéztek vagy automatikusan magasabb besorolással címkéztek.  További információ: [Az automatikus vagy ajánlott címkék alkalmazása](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Ha továbbra is problémákat tapasztal, gyűjtse össze az Azure Information Protection ügyfélnaplóit, és csatolja az exportált naplókat a támogatási jegyhez. Az Azure Information Protection naplóinak exportálásához:
    - Nyisson meg egy Office-dokumentumot, vagy hozzon létre egy új e-mailt az Outlookban.
    - Kattintson a **Védelem/Érzékenység** > **Súgó és visszajelzés** elemre.
    - Kattintson a **Naplók exportálása** gombra.
    - Mentse a naplókat a választott helyre, és csatolja őket a szolgáltatáskéréshez.

További információ:

- [Az Azure Information Protection automatikus és ajánlott besorolási feltételeinek konfigurálása](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Útmutatók az Azure Information Protection gyakori alkalmazási területeihez](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Az Azure Information Protection dokumentációjának áttekintése](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Az Azure Information Protection-előfizetések és -funkciók áttekintése](https://azure.microsoft.com/pricing/details/information-protection)
- [Az Azure Information Protection követelményei](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Rövid útmutató – Azure Information Protection – Oktatóanyag](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Az Azure Information Protection-ügyfél letöltése](https://www.microsoft.com/download/details.aspx?id=53018)
