---
title: A érzékenységi címkék nem jelennek meg
ms.author: stephow
author: stephow-MSFT
manager: laurawi
ms.date: ''
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 4bf8e02246c966f22648467386a7862f0521fecf
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207227"
---
# <a name="sensitivity-labels-not-appearing"></a>A érzékenységi címkék nem jelennek meg

A érzékenységi címkék lehetővé teszik a kényes tartalmak osztályozását és védelmét. Ők lehet teremtett-ban Mikroszkóp 365 engedékenység központ, Mikroszkóp 365 Biztonság Központ, vagy hivatal 365 biztonság & engedékenység központ alatt osztályozás > érzékenység felirat. A szolgáltatásról az [érzékenységi címkék áttekintése](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels)című témakör nyújt bővebb felvilágosítást.

Ha beállította az érzékenységi címkéket, de azok nem jelennek meg az Office-alkalmazásokban, ellenőrizze a következőket:

- Győződjön meg arról, hogy az érzékenységi címkét a kívánt felhasználók és csoportok számára [közzétették](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) .

- Ellenőrizze, hogy a felhasználó használ-e olyan alkalmazást, amely támogatja a érzékenységi címkéket – lásd: [érzékenységi címkék a dokumentumban](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable).

- Ha [áttelepíti a Azure adatvédelmet](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), vegye figyelembe az [itt](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)felsorolt szempontokat.

- Adatvesztés megelőzése (DLP) támogatás: jelenleg csak az adatmegőrzési címkéket lehet használni a DLP-házirendek feltételeként.  A DLP-házirend érzékenységi címkéinek támogatása még nem érhető el, de rajta dolgozunk.

- Ha egy érzékenységi címkén engedélyezve van a titkosítás, az alábbiak közül választhat:
    - Engedélyek hozzárendelése most
    - A felhasználók hozzárendeljék az engedélyeket


A lehetséges problémákról további információt a [érzékenységi címkékkel kapcsolatos ismert problémák](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc)című témakörben talál.