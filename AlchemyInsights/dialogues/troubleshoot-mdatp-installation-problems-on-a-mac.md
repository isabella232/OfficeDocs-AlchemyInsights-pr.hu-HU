---
title: Az MDATP telepítési problémáinak elhárítása Mac gépen
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694279"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Az MDATP telepítési problémáinak elhárítása Mac gépen

Ha a kézi  telepítés meghiúsul, a telepítővarázsló Összegzés lapján a következő hibaüzenet jelenik meg:

"Hiba történt a telepítés során. A telepítő hibát észlelt, amely a telepítés sikertelen voltát okozta. Segítségért forduljon a szoftver gyártójához."

A MDM-telepítések esetén a lapon általános telepítési hiba is látható.

Bár pontos hibákat nem jelenítünk meg a végfelhasználóknak, a telepítés előrehaladását egy naplófájlban tartjuk, a **/Library/Logs/Microsoft/mdatp/install.log** fájlban. Minden telepítési munkamenet hozzáfűzi ezt a naplófájlt. Ha csak az utolsó telepítési munkamenet kimenetét kimenetként, használja `sed` a .

További információt a Mac Microsoft Defender ATP telepítési [hibáinak elhárítása témakörben olvashat.](https://go.microsoft.com/fwlink/?linkid=2144615)
