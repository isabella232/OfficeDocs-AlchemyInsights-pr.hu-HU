---
title: A SharePoint-gyökérwebhely törlése
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
- "9003017"
- "5727"
ms.openlocfilehash: 4965e38f69c9d7f3a5c1facd23a0ee487e499f55f5779672808a54b86c90aeaa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102256"
---
# <a name="delete-the-sharepoint-root-site"></a>A SharePoint-gyökérwebhely törlése

A SharePoint-gyökérwebhely törlése **nem támogatott.**

1.  Ha a gyökérwebhelyet már törölték, a felhasználók 404-es, „A fájl nem található“ hibaüzenetet fognak kapni, amikor megpróbálnak hozzáférni a webhelyhez.
2.  A probléma megoldásához az új SharePoint Felügyeleti központból állítsa vissza a webhelyet azzal, hogy a [Törölt webhelyek](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) lapon kijelöli a gyökérwebhelyet, és a Visszaállítás lehetőségre kattint.
3.  A gyökérwebhely törlése helyett használja a [webhely cseréje](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site) lehetőséget az új SharePoint Felügyeleti központból a gyökérwebhely visszaállítása után.

További információért lásd: [A gyökérwebhely modernizálása](https://docs.microsoft.com/sharepoint/modern-root-site)