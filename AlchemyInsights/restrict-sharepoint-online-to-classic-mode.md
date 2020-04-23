---
title: A SharePoint Online klasszikus módra korlátozása
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: c5ea5d264b62e4c349623bd431776207b38da470
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742471"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>A SharePoint Online klasszikus módra korlátozása

Egyes szervezetektovábbra is megkövetelik a klasszikus mód élményt. Bár nem tervezi, hogy távolítsa el a klasszikus mód egy részletes szinten, már nem lehet korlátozni a teljes szervezet (bérlő) a klasszikus mód listák és tárak.

A rendszergazda a következő lehetőségekkel kezeli az egyes listákat és könyvtárakat klasszikus módban a következő szinteken biztosított részletes leiratkozási kapcsolókkal:

- webhelycsoport
- Oldalon
- Lista
- Könyvtár

Ezenkívül a modern által nem támogatott bizonyos funkciókat és testreszabásokat használó listák továbbra is automatikusan klasszikus módba váltanak.

2019. április 1-től a bérlői szint letiltásának folyamata elindul és folytatódik 2019. május 31-ig.  A bérlők letiltása miatt klasszikus módban lévő listák és tárak automatikusan átkerülnek a modern rendszerbe.

Ha klasszikus módra van szüksége, olvassa el a további információkat [itt](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) és a PnP Powershell utasítást [itt,](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) amely leírja a ma a klasszikus mód használatához használható lehetőségeket és eszközöket.
