---
title: Teljesítménybeli problémák SharePoint problémák OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 921aae7eba8487c5600f290fd671ef2675372e6af0478b913e38354856cbaa22
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911844"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint felhasználó OneDrive, nem érhető el vagy nem érhető el.

SharePoint vagy OneDrive lassú, elérhetetlen vagy nem érhető el, illetve a szolgáltatás elérhetetlenné válhat, illetve 503-as hiba jelenik meg több okból is:
  
- Ha az SharePoint- vagy OneDrive-webhelye lassú vagy késik több felhasználó esetén, átmeneti szolgáltatáshibát okozhat, amely miatt SharePoint felhasználók időnként késéseket vagy navigációs hibákat tapasztalhatnak OneDrive webhelyek elérésekor. Ellenőrizze a [Szolgáltatás állapota irányítópulton,](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) hogy nincs-e hatással a szervezete.
  
- Előfordulhat, hogy a felhasználók *503-as* kiszolgáló foglaltsági hibát kapnak, amikor megkísérelnek SharePoint vagy OneDrive webhelyre navigálni. Ezt a hibát a szolgáltatáson belüli SharePoint okozhatja. A SharePoint Online a szabályozást használja a SharePoint Online szolgáltatás optimális teljesítményének és megbízhatóságának fenntartásához. A szabályozás korlátozza a felhasználói műveletek vagy a párhuzamos hívások számát (parancsprogrammal vagy kóddal) az erőforrások túlzott felhasználásának megelőzése érdekében. A szabályozásról további információt A szabályozás elkerülése az online [SharePoint- SharePoint.](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- Ha egy klasszikus vagy  **modern** webhely vagy SharePoint lassú működést [](https://aka.ms/perftool) tapasztal, használja a Lapdiagnosztika eszközt a lapok elemzéséhez.
  
- Ha továbbra is általános lassú teljesítményt tapasztal, kérjük, tekintse át a következő cikk alján található forrásokat: Bevezetés a teljesítményhangolásba az SharePoint [Online-hoz](https://go.microsoft.com/fwlink/?linkid=2024334)
  