---
title: 'Példa: Microsoft Defender az Office 365 biztonságos mellékletekkel kapcsolatos házirendje'
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
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745994"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Példa: Microsoft Defender az Office 365 biztonságos mellékletekkel kapcsolatos házirendje

Ezek a beállítások engedélyezik a *Nincs* késés nevű házirendet, amely azonnal kézbesíti az üzeneteket, majd újra beolvassa a mellékleteket, miután beolvassa őket:

- **Név:** Nincs késés
- **Leírás:** Az üzenetek azonnali kézbesítése és a mellékletek újrafűzése a beolvasás után.
- **Válasz:** Válassza a **Dinamikus kézbesítés** lehetőséget. További információt a Dinamikus kézbesítés a Biztonságos mellékletek [házirendek esetén.](https://go.microsoft.com/fwlink/?linkid=2092328)
- Melléklet **átirányítása** szakasz: Válassza az Átirányítás engedélyezése lehetőséget, majd adja meg a Microsoft 365 globális rendszergazdájának, biztonsági rendszergazdájának vagy biztonsági elemzőnek az e-mail-címét, aki vizsgálja a kártékony mellékleteket.
- **Alkalmazott szakasz:** Válassza A **címzett tartománya lehetőséget,** majd válassza ki a tartományt. Válassza **a hozzáadás**, majd az OK **gombot.** Ha végzett, válassza a Mentés **gombot.**

További információt a Biztonságos mellékletek [az Office 365-hez](https://go.microsoft.com/fwlink/?linkid=2092213)való Microsoft Defenderben .
