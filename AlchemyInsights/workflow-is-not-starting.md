---
title: A munkafolyamat nem indul el
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 941e6349c98278a1a8cdac77457ec1cc72cdef8b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766099"
---
# <a name="workflow-is-not-starting"></a>A munkafolyamat nem indul el

- A SharePoint 2010 és a SharePoint 2013 munkafolyamatai nem indulnak el.

    - Ha a munkafolyamat nem indul el, előfordulhat, hogy ideiglenes szolgáltatásprobléma merül fel, amelyben a felhasználók időszakos késéseket tapasztalhatnak a munkafolyamat előrehaladásával. Ellenőrizze a [Szolgáltatásállapot-irányítópulton,](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) hogy a szervezet érintett-e.

    - Ha több mint 24 óra telt el azóta, hogy először látta ezt a problémát, kérjük, jelentkezzen be egy támogatási jegyet. Sok esetben már dolgozunk a megoldáson. Kérjük, adjon nekünk legalább 24 órát a megoldás befejezéséhez.

- A SharePoint 2010-munkafolyamatok elhúzódnak az indításkor.

    - Ez akkor fordul elő, ha a munkafolyamat nagy kötegekben aktiválódik. (például ha egyszerre több elemet ad hozzá).

    - A munkafolyamatokat nem valós idejű futtatásra tervezték, így a késleltetés a by-design viselkedése.

   -  Ha a munkafolyamat összetett Extensible Object Markup Language (XMOL), a fordítás lassú lehet. Ellenőrizze [ezt a](https://support.microsoft.com//kb/3043697) cikket.

    - Egyszerűsítse a munkafolyamatot, vagy tervezze újra a Microsoft SharePoint 2013 munkafolyamat-platformtípushasználatával.

    - Ha a munkafolyamat előzményei megnőttek, érdemes lehet kiüríteni az elemeket, vagy új előzménylistát létrehozni.

        További információ : [A munkafolyamat előzményeinek törlése](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Kapcsolódó témakörök
Kiszeretné próbálni a Microsoft Flow-t a SharePoint Online-ban?
- [Folyamat létrehozása](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint és Folyamat](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


