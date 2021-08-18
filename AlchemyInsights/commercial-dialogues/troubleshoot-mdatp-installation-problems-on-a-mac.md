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
ms.openlocfilehash: 4139f47f40a89069521aaa1a3e4fdab56e9e27a2096ae0ad099be827f60d51fc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091035"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Az MDATP telepítési hibáinak elhárítása Mac gépen

Ha nem sikerül a manuális telepítés, **a** telepítővarázsló Összegzés lapján a következő hibaüzenet jelenik meg:

"Hiba történt a telepítés során. A telepítő hibát észlelt, amely a telepítés sikertelen voltát okozta. Segítségért forduljon a szoftver gyártójához."

Az MDM-telepítések esetén a lapon egy általános telepítési hiba is látható.

Habár pontos hibákat nem jelenítünk meg a végfelhasználóknak, a telepítés előrehaladását a **/Library/Logs/Microsoft/mdatp/install.log** fájlban tartjuk. Minden telepítési munkamenet hozzáfűzi ezt a naplófájlt. Ha csak a legutóbbi telepítési munkamenet kimenetét kimenetként, használja a `sed` következőt: .

További információt A Mac Microsoft Defender ATP telepítési problémáinak elhárítása [témakörben olvashat.](https://go.microsoft.com/fwlink/?linkid=2144615)
