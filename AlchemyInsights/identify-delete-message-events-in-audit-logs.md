---
title: A naplókban szereplő üzenet-események törlésének felismerése
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696515"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Törölt e-mail-üzenetek naplózása

A 2019 januárban kezdődően a Microsoft alapértelmezés szerint bekapcsolja a postaláda-naplózást. Ellenkező esetben egy adott felhasználó törlési eseményeinek véleményezéséhez manuálisan kell engedélyeznie a naplózási műveleteket. Ha a postaláda naplózása már engedélyezve van a szervezetében vagy az adott felhasználónál, kövesse az alábbi lépéseket.

1. Jelentkezzen be a [Microsoft 365 biztonsági & megfelelőségi központjába](https://protection.office.com/) .

2. Kattintson a **Keresés és vizsgálat** elemre, és válassza a **naplózás keresése**lehetőséget.

3. Válassza ki a dátumtartomány értékét a **kezdési dátum** és a **Záró dátum** mezőben. Adja meg a vizsgálni kívánt felhasználó felhasználónevét (az elemeket törölt felhasználó). A **tevékenységek** mezőben válassza a törölt **elemek mappa törölt üzenetek** elemét, és **a törölt elemek mappába helyezi az üzeneteket**.

4. Kattintson a **Keresés**gombra.

A találatok között válasszon egy naplózási rekordot. Kattintson a részletek menü **További információk**parancsára. A törölt elemről (például a tárgyról és az elem törlési helyéről) további információk jelennek meg a **AffectedItems** mezőben. A **ClientInfoString** tulajdonság azt jeleníti meg, hogy a Törlés az Outlookban, a webes Outlookban (korábbi nevén Outlook Web App) vagy bármely más eszközön történt-e.

További tudnivalókat az [e-mail-továbbítás beállítása postaládához](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)című témakörben talál.

**Megjegyzés**: a törölt elemek nem olvashatók be a naplózási funkció használatával. A törölt üzenetek letöltéséhez a webes Outlookban lásd a [törölt elemek helyreállítása az Outlook Web App alkalmazásban](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)című témakört.
