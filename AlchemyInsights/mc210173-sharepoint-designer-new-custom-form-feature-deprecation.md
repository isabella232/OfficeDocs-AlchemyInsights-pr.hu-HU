---
title: MC210173 - SharePoint tervező új egyéni űrlaptulajdonság elavulása
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
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: 5be1ac4c8a4044adbc7d37c32ba7b3cb67c6cc25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831808"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a>MC210173 - SharePoint tervező új egyéni űrlaptulajdonság elavulása

Felfedeztünk egy olyan problémát, ami a SharePoint tervezőnek azt a funkcióját zavarja, ami az [egyéni űrlapokat hozza létre](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) a SharePoint online keretein belül. Egy alapos vizsgálatot követően megállapítottuk, hogy erre a problémára nincs ismert megoldás, ezért úgy döntöttünk, hogy 2020. április 25-én szombaton, az egyezményes koordinált világidő szerint hajnali 3 órától letiltjuk az egyéni űrlaplétrehozás funkciót. Ez a módosítás továbbra is engedi a korábban létrehozott űrlapok szerkesztését, és nem befolyásolja a SharePoint online tervező egyéb funkcióit.

A módosítást követően a felhasználók új űrlap létrehozása esetén a következő hibaüzenetet láthatják: „A lista változásai a szerverre nem menthetők”.

Azok a felhasználók, akik korábban a SharePoint tervezővel hoztak létre egyéni űrlapokat, a továbbiakban a [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) alkalmazást használhatják.

A PowerApps egy egyszerű és hatékony eszköz, amely lehetővé teszi, hogy a SharePoint online modern felületén működő felhasználók a SharePoint listák egyéni űrlapjait, illetve a dokumentumkönyvtárait közvetlenül a böngészőablakban hozzák létre, illetve szerkesszék. A PowerApps nem igényel hagyományos kódolási ismereteket, illetve speciális alkalmazásletöltéseket, mint amilyen, például az InfoPath.

**Megjegyzés**: A SharePoint Online Classic felhasználók ideiglenesen kapcsoljanak át a Modern felületre, hogy hozzáférhessenek és használhassák a PowerApps alkalmazást, habár a PowerApps alkalmazásban létrehozott valamennyi egyéni űrlap elérhető a SharePoint Online Classic felület használói számára is.
