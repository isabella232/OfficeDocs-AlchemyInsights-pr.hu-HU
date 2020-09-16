---
title: Nem jelennek meg a tartalmi Címkék
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
ms.openlocfilehash: 6a64e001be115c8e5553a0d8c97b8cb815922c69
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801186"
---
# <a name="sensitivity-labels-not-appearing"></a>Nem jelennek meg a tartalmi Címkék

A tartalmi címkék segítségével minősítheti és védheti a bizalmas tartalmakat. Ezek a Microsoft 365 megfelelőségi központban, a Microsoft 365 biztonsági központban vagy a Microsoft 365 biztonsági & megfelelőségi központban hozhatók létre > a tartalmi címkék osztályozása csoportban. A funkcióról a [tartalmi címkék áttekintése](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)című témakörben olvashat bővebben.

Ha beállította a tartalmi címkéit, de nem jelennek meg a Microsoft 365-alkalmazásokban, ellenőrizze az alábbiakat:

- Erősítse meg, hogy a tartalmi címkét [közzétették](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) a kívánt felhasználók és csoportok számára.

- Ellenőrizze, hogy a felhasználó egy olyan alkalmazást használ-e, amely támogatja a tartalmi címkéket – lásd: [a dokumentumban lévő tartalmi címkék](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).

- Ha Azure- [adatvédelemi címkéket szeretne áttelepíteni](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), ügyeljen az [itt](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)ismertetett szempontokra.

- Adatveszteség-megelőzés (DLP) támogatása: jelenleg csak az adatmegőrzési címkék használhatók feltételként a DLP-házirendekben.  Egy DLP-házirendben az érzékenységi címkék támogatása még nem érhető el, de éppen dolgozunk rajta.

- Ha a titkosítás engedélyezve van egy tartalmi címkén, az alábbiakra van lehetősége:
    - Engedélyek hozzárendelése most
    - Engedélyek hozzárendelése a felhasználókhoz


A lehetséges problémákról további információt az [érzékenységi címkék ismert problémái](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc)című témakörben talál.