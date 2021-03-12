---
title: Nem Windows rendszerű eszközök kitáblája a Microsoft Defender Komplex veszélyforrások elleni védelem (ATP) alkalmazásból
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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745647"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a>Nem Windows rendszerű eszközök kitáblája a Microsoft Defender Komplex veszélyforrások elleni védelem (ATP) alkalmazásból

Ezt a következőképpen teheti meg:

1. A harmadik féltől származó megoldás Microsoft Defender ATP-től való leválasztása érdekében kövesse a külső gyártó dokumentációját.
2. Az Azure Active Directory bérlői webhelyről távolítsa el a külső megoldás engedélyét:

    1. Jelentkezzen be az [Azure Portalba.](https://go.microsoft.com/fwlink/?linkid=2125612)
    1. Válassza **a Minden**  >  **szolgáltatás: Azure Active Directory**  >  **Nagyvállalati alkalmazások lehetőséget.**
    1. Jelölje ki azt az alkalmazást, amelyről ki szeretné választani a táblát.
    1. Válassza a **Törlés gombot.**

További információért olvassa el a Nem Windows rendszerű eszközök [ki vannak kapcsolva.](https://go.microsoft.com/fwlink/?linkid=2143630)
