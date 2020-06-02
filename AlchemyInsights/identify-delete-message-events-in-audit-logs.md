---
title: Üzenetesemények azonosítása a naplókban
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 641c0216491186aeb423a13854c6b39ee005e5df
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508990"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Törölt e-mail üzenetek naplóinak naplózása

2019 januárjától kezdve a Microsoft alapértelmezés szerint bekapcsolja a postaláda-naplózásnaplózást. Ellenkező esetben egy adott felhasználó üzeneteseményeinek ellenőrzéséhez manuálisan kell engedélyeznie a törlési műveleteket a naplózáshoz. Ha a postaláda naplózása már engedélyezve van a szervezetvagy az adott felhasználó számára, kövesse az alábbi lépéseket.

1. Bejelentkezés a [Microsoft 365 Biztonsági & megfelelőségi központjába](https://protection.office.com/)

2. Kattintson **a Keresés és vizsgálat** gombra, és válassza a **Naplókeresés lehetőséget.**

3. Válassza ki a dátumtartományt a **Kezdési dátum** és a **Záró dátum** mezőben. Adja meg a vizsgálni kívánt felhasználó (az elemeket törölt felhasználó) felhasználónevét. A **Tevékenységek** mezőben jelölje be a **Törölt üzenetek mappából a Törölt üzenetek mappából,** és **az Áthelyezett üzenetek mappába**.

4. Kattintson a **Keresés gombra.**

Az eredmények között jelöljön ki egy naplózási rekordot. A részletes úszó panelen kattintson a **További információ gombra.** A törölt cikkről (például a tárgysorról és a cikk törlésének helyéről) további információk jelennek meg az **Érintett elemek** mezőben. A **ClientInfoString** tulajdonság megmutatja, hogy a törlés megtörtént-e az Outlookban, a Webes Outlookban (korábbi nevén Outlook Web App) vagy bármely más eszközben.

További információt a [Postaláda e-mail-továbbítási beállításának meghatározása](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)című témakörben talál.

**Megjegyzés:** A naplószolgáltatás használatával nem lehet beolvasni a törölt elemeket. A törölt üzenetek beolvasása a Webes Outlookban a Törölt elemek helyreállítása az [Outlook Web Appban](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)című témakörben található.
