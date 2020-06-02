---
title: Az Office 365 Komplex veszélyforrások elleni védelemmel (ATP) kapcsolatos problémák elhárítása
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: f1dc675c8a8217ea2824ad46e029bfa303303e6a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511114"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a>Az Office 365 ATP-vel kapcsolatos problémák elhárítása

- **Értesítés késések e-mail üzenet kézbesítés?** Próbálja meg a dinamikus kézbesítési beállítást az ATP biztonságos mellékletek házirendjeihez. Ezzel elkerülhető késés az e-mailek kézbesítése, miközben megvédi a címzetteket a rosszindulatú fájloktól.
- **Hamis vagy hamis negatív okat szeretne jelenteni?** Ezen a hivatkozáson keresztül elküldheti a fájlt elemzésre:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)
- **Tudta, hogy engedélyezheti az ATP Safe Links védelmét a szervezeten belüli személyek között küldött e-mailek számára?** Hajtsa végre az alábbi lépéseket:
    1. Nyissa meg a https://protection.office.com t, és jelentkezzen be.
    2. Nyissa meg a **Fenyegetéskezelési**  >  **házirend**  >  **biztonságos hivatkozásait.**
    3. Az **adott címzettekre vonatkozó házirendek**csoportban szerkesztse (vagy adja hozzá) a házirendet.
    4. Jelölje be **A szervezeten belül küldött üzenetekre mutató biztonságos hivatkozások alkalmazása**jelölőnégyzetet.
    5. Mentse a szabályzatot, és hagyjon körülbelül 30 percet arra, hogy a módosítások végighaladjanak az adatközponton.
- Ha további segítségre van szüksége az ATP-vel kapcsolatban, olvassa el az [Office 365 Komplex veszélyforrások elleni védelem](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp)ben.