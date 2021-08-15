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
ms.openlocfilehash: fbaab348e06691b73db68492a0083c4a5a54c4504e03d27ec53f2a9f5047266d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53967803"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a>Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)

Ezt a következőképpen teheti meg:

1. A harmadik féltől származó megoldás Microsoft Defender ATP-től való leválasztása érdekében kövesse a külső gyártó dokumentációját.
2. A bérlői Azure Active Directory távolítsa el a külső megoldás engedélyét:

    1. Jelentkezzen be az [Azure portálra](https://go.microsoft.com/fwlink/?linkid=2125612).
    1. Válassza **a Minden szolgáltatás Azure Active Directory**  >    >  **Nagyvállalati alkalmazásokban lehetőséget.**
    1. Jelölje ki azt az alkalmazást, amelyről ki szeretné választani a táblát.
    1. Válassza a **Törlés gombot.**

További információért olvassa el a Ki vannak kapcsolva a nem Windows [eszközök.](https://go.microsoft.com/fwlink/?linkid=2143630)
