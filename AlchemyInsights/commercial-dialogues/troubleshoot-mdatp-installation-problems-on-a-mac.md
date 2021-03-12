---
title: Az MDATP telepítési hibáinak elhárítása Mac gépen
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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746302"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Az MDATP telepítési hibáinak elhárítása Mac gépen

Ha nem sikerül a manuális telepítés, **a** telepítővarázsló Összegzés lapján a következő hibaüzenet jelenik meg:

"Hiba történt a telepítés során. A telepítő hibát észlelt, amely a telepítés sikertelen voltát okozta. Segítségért forduljon a szoftver gyártójához."

Az MDM-telepítések esetén a lapon egy általános telepítési hiba is látható.

Habár pontos hibákat nem jelenítünk meg a végfelhasználóknak, a telepítés előrehaladását a **/Library/Logs/Microsoft/mdatp/install.log** fájlban tartjuk. Minden telepítési munkamenet hozzáfűzi ezt a naplófájlt. Ha csak a legutóbbi telepítési munkamenet kimenetét kimenetként, használja a `sed` következőt: .

További információt A Mac Microsoft Defender ATP telepítési problémáinak elhárítása [témakörben olvashat.](https://go.microsoft.com/fwlink/?linkid=2144615)
