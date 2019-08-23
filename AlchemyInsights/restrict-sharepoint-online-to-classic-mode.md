---
title: Klasszikus módú SharePoint Online korlátozása
ms.author: kirks
author: Techwriter40
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
ms.openlocfilehash: e7ecfd8c2f1a532355bfb8c2c0a846fc0d6e88b1
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551561"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>Klasszikus módú SharePoint Online korlátozása

Egyes szervezetek továbbra is csak a klasszikus mód tapasztalat. Nem tervezik alapszinten Klasszikus módú eltávolítása, amíg már nem korlátozhatja a klasszikus módban a listák és tárak teljes szervezeten (bérlő) lehetséges.

Az admin lesz egyéni listák és tárak klasszikus módban kapcsolókkal granulált lemondja, amit adunk a következő szinteken kezelheti a következők:

- webhelycsoport
- webhely
- lista
- dokumentumtár

Ezenkívül bizonyos szolgáltatásokat használó listák és modern által nem támogatott testreszabási beállításokat fogja továbbra is lehet automatikusan üzemmódba kell kapcsolni klasszikus.

Kezdődő április 1, 2019, a folyamat letiltása a bérlő szint befejezése mellett modern lista és könyvtárak elindítja, és folytassa a 2019 május 31-ig.  A listák és tárak, amelyek eredményeként a bérlő opt-out klasszikus módban a program automatikusan kell mozgatni, hogy a modern.

Ha a klasszikus módban van szüksége további információt talál [Itt](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) és a PnP Powershell instruction [Itt](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) , amely leírja a beállítások és eszközök segítségével ma a klasszikus módban felület használatára.
