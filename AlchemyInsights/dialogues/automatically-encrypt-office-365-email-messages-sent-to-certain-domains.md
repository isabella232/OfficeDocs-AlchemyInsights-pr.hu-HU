---
title: Bizonyos tartományoknak küldött Office 365-ös e-mailek automatikus titkosítása
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524876"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Bizonyos tartományoknak küldött Office 365-ös e-mailek automatikus titkosítása

1. Az [Exchange Felügyeleti központban válassza](https://outlook.office365.com/ecp/)az **e-mail-forgalomra > szabályokat.** 
2. Kattintson az **Új (+)** ikonra, majd az Office 365 Üzenettitkosítás és jogvédelem alkalmazása **az üzenetekre parancsra.**
3. A **Név** formában adja meg a szabály nevét, például a következő személynek küldött üzenetek *titkosítása contoso.com.*
4. A **Szabály alkalmazása, ha** a tartomány **címzettje >** lehetőséget. 
5. Írja be a tartomány nevét, például **contoso.com.**
6. Kattintson a **Hozzáadás (+)** ikonra, majd az **OK gombra.**
7. A Következő mező **mellett** kattintson az **Egyik kijelölése gombra.** 
8. Az **RmS sablon legördülő** menüjében válassza a Titkosítás **lehetőséget,** majd kattintson az **OK gombra.** (Ha nem látja ezt a lehetőséget, az azt jelenti, hogy a csomagja nem tartalmaz automatikus titkosítást. De hozzáadhatja!)
9. Tetszőlegesen választhat (az ezen a ponton választható választható beállítások listájából, amelyek közül sok az egyszerűség alapértelmezett beállításával hagyható meg).
10. Kattintson a **Mentés** gombra.

> [!IMPORTANT]
> Később mindig visszajöhet, és szerkesztheti ezt a szabályt.

További információ a titkosítási szabályok létrehozásáról: E-mail-forgalom szabályainak meghatározása az e-mailek titkosításához az [Office 365-ben](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)