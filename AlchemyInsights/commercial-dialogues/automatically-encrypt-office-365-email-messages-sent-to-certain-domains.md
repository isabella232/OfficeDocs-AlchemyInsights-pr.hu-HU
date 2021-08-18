---
title: Bizonyos tartományokra Office 365 küldött e-mailek automatikus titkosítása
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
ms.openlocfilehash: d30535d8605fcbfa0ca73c262d8f8671d73234a4
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318850"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Bizonyos tartományokra Office 365 küldött e-mailek automatikus titkosítása

1. A Felügyeleti [Exchange felügyeleti központban válassza](https://outlook.office365.com/ecp/)az **e-mail-forgalom és > lehetőséget.** 
2. Kattintson az **Új (+)** ikonra, majd a Szövegvédelem Office 365 Üzenettitkosítás és jogvédelem alkalmazása **az üzenetekre elemre.**
3. A **Név** formában adja meg a szabály nevét, például a következőnek küldött üzenetek *titkosítása contoso.com.*
4. A **Szabály alkalmazása, ha területen** válassza A címzett és > **lehetőséget.** 
5. Írja be a tartomány nevét, például **contoso.com.**
6. Kattintson **a Hozzáadás (+)** ikonra, majd az **OK gombra.**
7. A következő **lépés mező mellett** kattintson a Válasszon **gombra.** 
8. Az **RMS sablon legördülő** menüjében válassza a **Titkosítás** elemet, majd kattintson az **OK gombra.** (Ha nem látja ezt a beállítást, az azt jelenti, hogy a csomagja nem tartalmaz automatikus titkosítást. De ön is hozzáadhatja!)
9. Válasszon a választható beállítások közül (az ezen a ponton választható beállítások listájából, amelyek közül sok az egyszerűség alapértelmezett beállításával hagyható meg).
10. Kattintson a **Mentés** gombra.

**Fontos:** Később mindig visszahozhatja és szerkesztheti ezt a szabályt.

A titkosítási szabályok létrehozásáról további információt az [E-mail-forgalom](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) szabályainak megadása az e-mailek titkosításához a Office 365