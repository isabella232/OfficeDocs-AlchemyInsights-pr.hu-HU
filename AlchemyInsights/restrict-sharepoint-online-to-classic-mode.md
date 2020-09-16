---
title: A SharePoint Online és a klasszikus üzemmód korlátozása
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751424"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>A SharePoint Online és a klasszikus üzemmód korlátozása

Egyes szervezetek esetében továbbra is szükség van a klasszikus üzemmódra. Noha a klasszikus üzemmód nem távolítható el egy szemcsés szinten, a listák és tárak számára már nem korlátozható a teljes szervezet (bérlő) a klasszikus módra.

A rendszergazda az alábbi lépésekkel kezelheti az egyes listákat és tárakat az alábbi szinteken:

- webhelycsoport
- webhely
- lista
- tár

Ezenkívül a modern funkció által nem támogatott funkciókat és testreszabásokat használó listák továbbra is automatikusan klasszikus módra váltanak.

Április 1-től kezdődően az 2019, a bérlői szint letiltásának folyamata letilthatja a modern listák és tárak közötti indulást, és az 2019 május 31-én folytatódik.  A bérlői opt-out-ban klasszikus módban lévő listák és tárak automatikusan a modern verzióba kerülnek.

Ha klasszikus üzemmódra van szüksége, olvassa el a további információ [itt](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) és a PnP PowerShell-utasítások című témakört, amely [bemutatja, hogy](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) miként használhatja a mai naptól a klasszikus mód használatát.
