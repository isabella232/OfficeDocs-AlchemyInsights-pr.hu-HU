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
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403745"
---
# <a name="workflow-is-not-starting"></a>Nem indul el a munkafolyamat

- A SharePoint 2010-es és a SharePoint 2013-as munkafolyamatok nem indulnak el.

    - Ha a munkafolyamat nem indul el, átmeneti szolgáltatás-probléma lehet, amely miatt a felhasználók időnként késéseket tapasztalhatnak a munkafolyamat előrehaladásával. Ellenőrizze a [Szolgáltatás állapota irányítópulton,](https://admin.microsoft.com/AdminPortal/Home/servicehealth) hogy nincs-e hatással a szervezete.

    - Ha a probléma első jelentkezte óta több mint 24 óra telt el, kérjük, írjon be egy támogatási jegyet. Sok esetben már dolgozunk a megoldáson. Kérjük, várjon legalább 24 órát a megoldásunkra.

- A SharePoint 2010-munkafolyamatok késleltetve vannak az indítás során.

    - Ez akkor fordul elő, ha a munkafolyamatot nagy kötegek indítják el. (ha például egyszerre több elemet ad hozzá).

    - A munkafolyamatok nem valós idejű futtatásra vannak tervezve, ezért a késés szándékos működés.

   -  Ha a Munkafolyamat összetett Extensible Object Markup Language (XALBUM), az összeállítás lassú lehet. Ellenőrizze [ezt a](https://support.microsoft.com//kb/3043697) cikket.

    - Egyszerűsítse vagy tervezse újra a munkafolyamatot a Microsoft SharePoint 2013 munkafolyamat-platformtípusának használatával.

    - Ha a munkafolyamat előzményei egyre nagyobbak, előfordulhat, hogy véglegesen szeretné véglegesen létrehozni az elemeket, vagy új előzményeket szeretne létrehozni.

        További információ: [Munkafolyamat előzményeinek végleges végleges módosítása](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Kapcsolódó témakörök
Szeretné kipróbálni a Microsoft Flow-t a SharePoint Online-ban?
- [Folyamat létrehozása](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint és Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
