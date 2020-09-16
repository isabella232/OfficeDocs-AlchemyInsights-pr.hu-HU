---
title: Az Office terminálkiszolgálón való telepítésekor felmerülő problémák megoldása
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 85f24284-af6f-4624-b6be-901a4a9206eb
ms.openlocfilehash: df1a50031196fbd79662cee620fc41c7be14e179
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47738459"
---
# <a name="solutions-for-issues-around-installing-office-on-a-terminal-server"></a>Az Office terminálkiszolgálón való telepítésekor felmerülő problémák megoldása

A megosztott számítógép-aktiválás használatához olyan előfizetéssel kell rendelkeznie, amely magában foglalja a Microsoft 365-alkalmazásokat a nagyvállalatoknak.
  
- Annak ellenőrzése, hogy engedélyezve van-e a megosztott számítógép aktiválása
- Az aktiválás sikerességének ellenőrzése
- A megosztott számítógép aktiválásával kapcsolatos hibaüzenetek áttekintése:
- "A fiókjában talált termékek nem használhatók az Office aktiválásához megosztott számítógépeken"
  
Ez a hibaüzenet azt jelzi, hogy nincs olyan előfizetése, amely tartalmazza a Microsoft 365-alkalmazásokat a nagyvállalatoknak.

"Nem licencelt termék"

- Ellenőrizze, hogy a felhasználóhoz van-e hozzárendelve licenc a Microsoft 365-alkalmazások nagyvállalati verzióhoz.
- Ellenőrizze, hogy a felhasználó bejelentkezik-e a felhasználói fiókjával.
- Ellenőrizze, hogy van-e kapcsolat a megosztott számítógép és az internet között.

További hibaelhárítási tippekért lásd: [a megosztott számítógép aktiválásával kapcsolatos problémák elhárítása](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)