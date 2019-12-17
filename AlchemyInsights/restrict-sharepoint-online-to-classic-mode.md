---
title: A SharePoint Online klasszikus üzemmódra korlátozása
ms.author: pebaum
author: pebaum
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: b58a1c3fc331c739080542917d8945c090ec0d94
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048762"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>A SharePoint Online klasszikus üzemmódra korlátozása

Egyes szervezeteknél továbbra is klasszikus üzemmódra van szükség. Bár nem tervezi, hogy távolítsa el a klasszikus mód a szemcsés szinten, már nem lehet korlátozni egy egész szervezet (bérlő) a klasszikus mód listák és tárak.

A admin akarat volna a következő választások-hoz kezel egyén tetszik és könyvtárak-ban klasszikus mód használ szemcsés választ-ki kapcsol amit mi beszerez-nél alábbiak szintek:

- webhelycsoport
- Oldalon
- Lista
- Könyvtár

Továbbá azok a listák, amelyek bizonyos szolgáltatásokat és testreszabásokat használnak, amelyeket a modern nem támogat, továbbra is automatikusan klasszikus módra lesznek átkapcsolva.

Kezdet április 1, 2019, a folyamat-hoz megbénít a bérlő szinten opt out a modern lista és könyvtárak indul, és továbbra is a május 31, 2019.  Azok a listák és könyvtárak, amelyek klasszikus módban vannak bérlő opt-out eredményeként automatikusan eltolódnak a modern.

Ha klasszikus üzemmódra van szüksége, olvassa el a további tudnivalókat [itt](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) , és a PnP PowerShell instrukció [itt](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) leírja azokat a lehetőségeket és eszközöket, amelyeket ma használhat a klasszikus üzemmód használatához.
