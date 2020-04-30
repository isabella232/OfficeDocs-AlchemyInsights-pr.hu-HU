---
title: MC210173 - SharePoint tervező új egyéni űrlaptulajdonság elavulása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: 185e8fc94345b240667490b1ffc63af8459d8daf
ms.sourcegitcommit: a9e6b2fcce8bd12fd079ed967f426b67d5c6d239
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43928530"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a>MC210173 - SharePoint tervező új egyéni űrlaptulajdonság elavulása

Felfedeztünk egy olyan problémát, ami a SharePoint tervezőnek azt a funkcióját zavarja, ami az [egyéni űrlapokat hozza létre](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) a SharePoint online keretein belül. Egy alapos vizsgálatot követően megállapítottuk, hogy erre a problémára nincs ismert megoldás, ezért úgy döntöttünk, hogy 2020. április 25-én szombaton, az egyezményes koordinált világidő szerint hajnali 3 órától letiltjuk az egyéni űrlaplétrehozás funkciót. Ez a módosítás továbbra is engedi a korábban létrehozott űrlapok szerkesztését, és nem befolyásolja a SharePoint online tervező egyéb funkcióit.

A módosítást követően a felhasználók új űrlap létrehozása esetén a következő hibaüzenetet láthatják: „A lista változásai a szerverre nem menthetők”.

Azok a felhasználók, akik korábban a SharePoint tervezővel hoztak létre egyéni űrlapokat, a továbbiakban a [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) alkalmazást használhatják.

A PowerApps egy egyszerű és hatékony eszköz, amely lehetővé teszi, hogy a SharePoint online modern felületén működő felhasználók a SharePoint listák egyéni űrlapjait, illetve a dokumentumkönyvtárait közvetlenül a böngészőablakban hozzák létre, illetve szerkesszék. A PowerApps nem igényel hagyományos kódolási ismereteket, illetve speciális alkalmazásletöltéseket, mint amilyen, például az InfoPath.

**Megjegyzés**: A SharePoint Online Classic felhasználók ideiglenesen kapcsoljanak át a Modern felületre, hogy hozzáférhessenek és használhassák a PowerApps alkalmazást, habár a PowerApps alkalmazásban létrehozott valamennyi egyéni űrlap elérhető a SharePoint Online Classic felület használói számára is.
