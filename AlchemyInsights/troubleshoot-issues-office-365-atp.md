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
ms.openlocfilehash: 99bc985f2d66693aca45f0833ab47c043acc1324
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766747"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a>Az Office 365 ATP-vel kapcsolatos problémák elhárítása

- **Értesítés késések e-mail üzenet kézbesítés?** Próbálja meg a dinamikus kézbesítési beállítást az ATP biztonságos mellékletek házirendjeihez. Ezzel elkerülhető késés az e-mailek kézbesítése, miközben megvédi a címzetteket a rosszindulatú fájloktól.
- **Hamis vagy hamis negatív okat szeretne jelenteni?** Ezen a hivatkozáson keresztül elküldheti a fájlt elemzésre:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)
- **Tudta, hogy engedélyezheti az ATP Safe Links védelmét a szervezeten belüli személyek között küldött e-mailek számára?** Hajtsa végre az alábbi lépéseket:
    1. Nyissa https://protection.office.commeg a t, és jelentkezzen be.
    2. Nyissa meg a **Fenyegetéskezelési** > **házirend** > **biztonságos hivatkozásait.**
    3. Az **adott címzettekre vonatkozó házirendek**csoportban szerkesztse (vagy adja hozzá) a házirendet.
    4. Jelölje be **A szervezeten belül küldött üzenetekre mutató biztonságos hivatkozások alkalmazása**jelölőnégyzetet.
    5. Mentse a szabályzatot, és hagyjon körülbelül 30 percet arra, hogy a módosítások végighaladjanak az adatközponton.
- Ha további segítségre van szüksége az ATP-vel kapcsolatban, olvassa el az [Office 365 Komplex veszélyforrások elleni védelem](https://docs.microsoft.com/office365/securitycompliance/office-365-atp)ben.