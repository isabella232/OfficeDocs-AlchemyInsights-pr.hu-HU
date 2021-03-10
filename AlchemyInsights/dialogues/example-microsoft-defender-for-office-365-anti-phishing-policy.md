---
title: Példa az Office 365-nek az adathalászat elleni védelemre vonatkozó Microsoft Defenderre
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
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694036"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Példa az Office 365-nek az adathalászat elleni védelemre vonatkozó Microsoft Defenderre

Ezek a beállítások engedélyezik a Domain and CEO (Tartomány és *igazgató) házirendet.* Ez a házirend biztosítja a felhasználók és a tartományok védelmét a megszemélyesítés ellen, majd a tartományon belüli felhasználóktól kapott összes e-mailre alkalmazza a házirendet. Először adja hozzá az alábbi adatokat a házirend létrehozásához:

- **Név:** Domain and CEO **Description**: Ensures that the CEO and your domain are not impersonated.
  **Alkalmazva:** Jelölje **ki a címzett tartományát.** A **Válasszon, majd válasszon** egy tartományt a Beállítások csoportban.  Válassza **a + Hozzáadás gombot.** Jelölje be a listában a tartomány neve melletti jelölőnégyzetet (például *contoso.com),* majd válassza az **Add (Hozzáadás) lehetőséget.** Válassza **a Kész gombot.**
- A házirend létrehozása után a következő beállításokkal finomhangolhatja a házirendet:
  - **Felhasználók hozzáadása védelemhez:** Ebben a példában adja meg legalább az igazgató e-mail-címét.
  - **Tartományok hozzáadása védelemhez:** Vegye fel azt a szervezeti tartományt, amely tartalmazza az ügyvezető igazgató irodáját.
  - **Válassza ki a** műveleteket: Ha egy megszemélyesített felhasználó küldi az e-mailt, válassza az Üzenet átirányítása másik e-mail címre **lehetőséget,** majd adja meg a biztonsági rendszergazda *e-mail-címét*(például securityadmin@contoso.com). Ha **megszemélyesített** tartomány küldi az e-maileket, válassza az üzenet **karanténba való kijelölését.**
  - **Postaláda-intelligencia:** Ez a beállítás alapértelmezés szerint be van jelölve új adathalászati házirend létrehozásakor. A legjobb eredmény érdekében hagyja **be** ezt a beállítást.
  - **Megbízható feladók és tartományok hozzáadása:** Ebben a példában ne definiálja a felülbírálásokat.
- Miután átnézte a beállításokat,  válassza a Házirend létrehozása vagy **a Mentés** lehetőséget a megfelelő módon.

További információt az adathalászat elleni házirendek [a Microsoft 365-ben.](https://go.microsoft.com/fwlink/?linkid=2092235)
