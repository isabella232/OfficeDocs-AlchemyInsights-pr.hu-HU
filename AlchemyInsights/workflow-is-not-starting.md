---
title: Nem indul el a munkafolyamat
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794769"
---
# <a name="workflow-is-not-starting"></a>Nem indul el a munkafolyamat

- A SharePoint 2010 és a SharePoint 2013-munkafolyamatok nem indulnak el.

    - Ha a munkafolyamata nem indul el, lehet, hogy ideiglenes szolgáltatási problémát tapasztal, ahol a felhasználók időnként késleltetni fogják a munkafolyamatok állapotát. A [szolgáltatás állapota irányítópulton](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) ellenőrizheti, hogy a szervezete hatással van-e rá.

    - Ha több mint 24 óra telt el, mióta először látta ezt a problémát, kérjük, jelentkezzen be egy támogatási jegybe. Sok esetben már dolgozunk a megoldáson. Kérjük, hogy végezze el a megfelelő megoldást legalább 24 óráig.

- A SharePoint 2010-munkafolyamatai a kezdőképernyőn késleltetve jelennek meg.

    - Ez akkor fordul elő, ha a munkafolyamatot nagy kötegekben indítja el. (például ha egyszerre több elemet adott meg).

    - A munkafolyamatok nem futtathatók valós időben, ezért a késések a tervezés viselkedését szolgálják.

   -  Ha a munkafolyamat összetett Extensible Object Markup Language (XMOL), a fordítás lassú lehet. Olvassa el [ezt a](https://support.microsoft.com//kb/3043697) cikket.

    - Egyszerűsíteni kell a munkafolyamatot, vagy át kell terveznie a Microsoft SharePoint 2013 munkafolyamat-platform típusa használatával.

    - Ha a munkafolyamat előzményei nagyban nőttek, érdemes lehet törölni az elemeket, vagy létre kell hoznia egy új előzményeket tartalmazó listát.

        További információ: [munkafolyamat-előzmények törlése](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Kapcsolódó témakörök
Szeretné kipróbálni a Microsoft flow-t a SharePoint Online-ban?
- [Folyamatábra létrehozása](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint és flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


