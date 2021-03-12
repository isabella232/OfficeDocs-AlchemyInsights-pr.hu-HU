---
title: Bizonyos tartományokra küldött Office 365-ös e-mailek automatikus titkosítása
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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746050"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Bizonyos tartományokra küldött Office 365-ös e-mailek automatikus titkosítása

1. Az [Exchange Felügyeleti központban válassza](https://outlook.office365.com/ecp/)az **e-mail-forgalom és > lehetőséget.** 
2. Kattintson az **Új (+)** ikonra, majd az **Office 365** Üzenettitkosítás és jogvédelem alkalmazása az üzenetekre elemre.
3. A **Név** formában adja meg a szabály nevét, például a következőnek küldött üzenetek *titkosítása contoso.com.*
4. A **Szabály alkalmazása, ha területen** válassza A címzett > **lehetőséget.** 
5. Írja be a tartomány nevét, például **contoso.com.**
6. Kattintson **a Hozzáadás (+)** ikonra, majd az **OK gombra.**
7. A következő **lépés mező mellett** kattintson a Válasszon **gombra.** 
8. Az **RMS sablon legördülő** menüjében válassza a **Titkosítás** elemet, majd kattintson az **OK gombra.** (Ha nem látja ezt a beállítást, az azt jelenti, hogy a csomagja nem tartalmaz automatikus titkosítást. De ön is hozzáadhatja!)
9. Válasszon a választható beállítások közül (az ezen a ponton választható beállítások listájából, amelyek közül sok az egyszerűség alapértelmezett beállításával hagyható meg).
10. Kattintson a **Mentés** gombra.

> [!IMPORTANT]
> A szabályt később is mindig módosíthatja.

A titkosítási szabályok létrehozásáról további információt az E-mail-forgalom szabályainak megadása az [Office 365-ben](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) az e-mailek titkosításához