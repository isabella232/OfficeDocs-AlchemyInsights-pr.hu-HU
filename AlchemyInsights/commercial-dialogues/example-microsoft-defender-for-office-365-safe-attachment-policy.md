---
title: Példa a Microsoft Defender Office 365 Széf mellékletre vonatkozó házirendhez
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
ms.openlocfilehash: 7294be81a24fa61a92367bae304798a333cb916c8718e28b1a87314c15ef6c8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988297"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Példa a Microsoft Defender Office 365 Széf mellékletre vonatkozó házirendhez

Ezek a beállítások engedélyezik a *Nincs* késés nevű házirendet, amely azonnal kézbesíti az üzeneteket, majd újra beolvassa a mellékleteket, miután beolvassa őket:

- **Név:** Nincs késés
- **Leírás:** Az üzenetek azonnali kézbesítése és a mellékletek újrafűzése a beolvasás után.
- **Válasz:** Válassza a **Dinamikus kézbesítés** lehetőséget. További információ: Dinamikus kézbesítés a Széf [házirendek esetén.](https://go.microsoft.com/fwlink/?linkid=2092328)
- **Mellékletek átirányítása** szakasz: Válassza az Átirányítás engedélyezése lehetőséget, majd adja meg az Microsoft 365 globális rendszergazdájának, biztonsági rendszergazdájának vagy biztonsági elemzőnek az e-mail-címét, aki vizsgálja a kártékony mellékleteket.
- **Alkalmazott szakasz:** Válassza A **címzett tartománya lehetőséget,** majd válassza ki a tartományt. Válassza **a hozzáadás**, majd az OK **gombot.** Ha végzett, válassza a Mentés **gombot.**

További információt a Mellékletek Széf [a Microsoft Defender for Office 365.](https://go.microsoft.com/fwlink/?linkid=2092213)
