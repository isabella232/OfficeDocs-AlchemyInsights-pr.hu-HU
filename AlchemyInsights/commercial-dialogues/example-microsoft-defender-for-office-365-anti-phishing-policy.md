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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746855"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Példa az Office 365-nek az adathalászat elleni védelemre vonatkozó Microsoft Defenderre

Ezek a beállítások engedélyezik a Domain and CEO (Tartomány és *igazgató) nevű házirendet.* Ez a házirend a felhasználók és a tartományok megszemélyesítése elleni védelmet is biztosítja, majd a tartományon belüli felhasználóktól kapott összes e-mailre alkalmazza a házirendet. Először adja hozzá a következő információkat a házirend létrehozásához:

- **Név:** Domain and CEO Description : **Biztosítja,** hogy a CEO-t és a tartományt ne személyesítették meg.
  **Alkalmazva:** A **címzett tartományának kijelölése:**. A **Válasszon egyet csoportban válassza** a Choose **(Választás)** lehetőséget, majd válasszon egy tartományt. Válassza **a + Hozzáadás lehetőséget.** Jelölje be a listában a tartomány neve melletti jelölőnégyzetet (például contoso.com *),* majd válassza a **Hozzáadás lehetőséget.** Válassza a **Kész lehetőséget.**
- A házirend létrehozása után az alábbi beállításokkal finomhangolhatja a házirendet:
  - **Felhasználók hozzáadása védelemhez:** Ebben a példában vegye fel legalább az ügyvezető igazgató e-mail-címét.
  - **Védjen meg tartományokat:** Vegye fel azt a szervezeti tartományt, amely tartalmazza az ügyvezető igazgató irodáját.
  - Műveletek **kiválasztása:** Ha egy megszemélyesített felhasználó küldött e-mailt, válassza az Üzenet átirányítása másik e-mail címre **lehetőséget,** majd adja meg a biztonsági rendszergazda *e-mail-címét (például securityadmin@contoso.com).* Ha **megszemélyesített** tartomány küldi az e-maileket, válassza az Üzenet **karanténba küldése lehetőséget.**
  - Postaláda-intelligencia: Új adathalászat-házirend létrehozásakor ez a beállítás alapértelmezés szerint be van jelölve. A legjobb eredmény érdekében hagyja **be a** beállítást.
  - **Megbízható feladók és tartományok hozzáadása:** Ebben a példában ne definiálja a felülbírálásokat.
- A beállítások áttekintése után válassza  a Házirend létrehozása vagy a **Mentés** lehetőséget a megfelelő módon.

További információ: [Adathalászat elleni házirendek a Microsoft 365-ben.](https://go.microsoft.com/fwlink/?linkid=2092235)
