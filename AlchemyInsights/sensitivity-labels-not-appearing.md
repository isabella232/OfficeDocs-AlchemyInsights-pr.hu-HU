---
title: Nem jelennek meg a bizalmasság-címkék
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 824824257fee4aaaab1f2dd32597b4cdc858d035fabd357af90cf054dd35c9c4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061434"
---
# <a name="sensitivity-labels-not-appearing"></a>Nem jelennek meg a bizalmasság-címkék

A bizalmas tartalomcímkék segítségével osztályozhatja és megvédheti bizalmas tartalmait. A besorolási és bizalmasségi címkék Microsoft 365 Megfelelőségi központ, Microsoft 365 vagy Microsoft 365 > megfelelőségi központban & osztályban lehet létrehozni őket. A funkcióról további információt A bizalmasság-címkék [áttekintése témakörben talál.](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)

Ha konfigurálta a bizalmasság-címkéket, de azok nem jelennek meg a Microsoft 365 appokban, ellenőrizze az alábbiakat:

- Győződjön meg arról, hogy [](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) a bizalmasság címkéje közzé lett tett a kívánt felhasználóknak és csoportoknak.

- Győződjön meg arról, hogy a felhasználó egy olyan alkalmazást használ, amely támogatja a bizalmasság-címkéket – lásd a bizalmasság-címkéket [a dokumentumban.](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable)

- Ha Azure [Information Protection-címkéket](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)áttelepítésekor figyelembe kell vennie az itt felsorolt [szempontokat.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)

- Adatveszteség-megelőzési (DLP) támogatás: Jelenleg csak az adatmegőrzési címkék használhatók feltételként a DLP-házirendben.  A bizalmasság-megelőzési házirendek támogatása még nem érhető el, de dolgozunk rajta.

- Ha a titkosítás engedélyezve van egy bizalmasság-címkén, a következő beállítások közül választhat:
    - Engedélyek hozzárendelése most
    - Engedélyek hozzárendelésének lehetővé teszi a felhasználók számára


A lehetséges problémákról további információt az Ismert [problémák a bizalmasság-címkékkel kapcsolatban.](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc)