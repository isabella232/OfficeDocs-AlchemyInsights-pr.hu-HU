---
title: A meglévő böngészőkörnyezet értékelése és a célok meghatározása
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9141"
- "9005291"
ms.openlocfilehash: 5b03d188aa78be83928cf262f1d86f3f933c85ab
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693640"
---
# <a name="evaluate-your-existing-browser-environment-and-define-goals"></a>A meglévő böngészőkörnyezet értékelése és a célok meghatározása

A böngésző jelenlegi állapotának és a projektlátásnak a segítségével biztosíthatja, hogy a projekt minden érintettje egy vonalban van, és ugyanazon cél érdekében dolgoznak. Hajtsa végre az alábbi lépéseket:

1. Határozza meg az aktuális állapotot. Célszerű megemlíteni az alábbiakat:
- Jelenleg mely böngészők vannak telepítve a környezetében?
- Melyik böngésző van beállítva alapértelmezett böngészőként?
- Szüksége van az Internet Explorerre néhány alkalmazáshoz?
- Vállalati módú webhelylistát használ az Internet Explorer beállításához?
- Mely operációs rendszerek (például a Windows 10 és a macOS) támogatottak a környezetében?
- Milyen kezelőeszközöket használ a böngésző kezeléséhez?
- Ki a felelős a böngészők konfigurációáért és kezeléséért?
- Milyen folyamattal érvényesíthető a böngészőkompatibilitás?
2. Határozza meg a telepítés céljait. Tartsa szem előtt az alábbiakat:
- Be szeretné állítani a [Microsoft Edge-et alapértelmezett böngészőként?](https://docs.microsoft.com/DeployEdge/edge-default-browser)
- Szeretné elrejteni a Microsoft Edge régi verzióját, vagy elérhetővé szeretné tenni a [felhasználóknak?](https://docs.microsoft.com/DeployEdge/microsoft-edge-sysupdate-access-old-edge)
- Hogyan fogja [konfigurálni a Microsoft Edge-et?](https://docs.microsoft.com/DeployEdge/configure-microsoft-edge)
- Milyen funkciókat kell konfigurálni a kezdeti telepítés részeként?
- Milyen folyamat során történik az azonosított kompatibilitási vagy konfigurációs problémák megoldása?
3. A funkciók használatának előfeltételei, például:
- [Windows Defender alkalmazásőr](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-application-guard/reqs-md-app-guard)
- [Internet Explorer mód](https://docs.microsoft.com/DeployEdge/edge-ie-mode)
- [Hitelesítés és szinkronizálás](https://docs.microsoft.com/DeployEdge/microsoft-edge-security-identity)

A lépések végrehajtása után készen áll az üzembe helyezési stratégia megtervezésére.
