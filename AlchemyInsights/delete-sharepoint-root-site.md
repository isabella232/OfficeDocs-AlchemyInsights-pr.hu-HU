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
ms.openlocfilehash: 849c5c58ab4688130d71baffac8fe39eddf92f18
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815473"
---
# <a name="delete-the-sharepoint-root-site"></a>A SharePoint-gyökérwebhely törlése

A SharePoint-gyökérwebhely törlése **nem támogatott.**

1.  Ha a gyökérwebhelyet már törölték, a felhasználók 404-es, „A fájl nem található“ hibaüzenetet fognak kapni, amikor megpróbálnak hozzáférni a webhelyhez.
2.  A probléma megoldásához az új SharePoint Felügyeleti központból állítsa vissza a webhelyet azzal, hogy a [Törölt webhelyek](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) lapon kijelöli a gyökérwebhelyet, és a Visszaállítás lehetőségre kattint.
3.  A gyökérwebhely törlése helyett használja a [webhely cseréje](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site) lehetőséget az új SharePoint Felügyeleti központból a gyökérwebhely visszaállítása után.

További információért lásd: [A gyökérwebhely modernizálása](https://docs.microsoft.com/sharepoint/modern-root-site)