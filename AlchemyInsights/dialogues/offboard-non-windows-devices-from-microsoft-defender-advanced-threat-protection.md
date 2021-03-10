---
title: Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)
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
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693815"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a>Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)

Ezt a következőképpen teheti meg:

1. A harmadik féltől származó megoldás Microsoft Defender ATP-ről való leválasztása érdekében kövesse a külső gyártó dokumentációját.
2. Az Azure Active Directory-bérlőből távolítsa el a külső megoldás engedélyét:

    1. Jelentkezzen be az [Azure Portalba.](https://go.microsoft.com/fwlink/?linkid=2125612)
    1. Válassza **az Azure** Active Directory Enterprise Applications összes  >    >  **szolgáltatását.**
    1. Jelölje ki azt az alkalmazást, amelyről ki szeretné választani a táblát.
    1. Válassza a **Törlés gombot.**

További információért olvassa el a nem Windows rendszerű eszközök [kitáblás eszközeit.](https://go.microsoft.com/fwlink/?linkid=2143630)
