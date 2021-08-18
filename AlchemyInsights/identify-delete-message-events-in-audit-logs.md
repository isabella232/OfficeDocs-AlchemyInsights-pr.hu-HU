---
title: A naplók törlési üzeneteseményének azonosítása
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
ms.openlocfilehash: f5d6041fd80b4d5cae610e7d9248e45ed410a3d9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317596"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Törölt e-mailek naplói

2019 januártól kezdődően a Microsoft alapértelmezés szerint bekapcsolja a postaláda-naplózást. Ha egy adott felhasználó törlési eseményeit szeretné áttekintani, manuálisan engedélyeznie kell a naplózáshoz szükséges törlési műveleteket. Ha a postaláda-naplózás már engedélyezve van a szervezet vagy az adott felhasználó számára, kövesse az alábbi lépéseket.

1. Bejelentkezés az [Microsoft 365 megfelelőségi központba](https://protection.office.com/)

2. Kattintson **a Keresés és vizsgálat elemre,** és válassza a **Naplókeresés lehetőséget.**

3. Jelölje ki a dátumtartományt a **Kezdő dátum és** a Záró dátum **mezőben.** Adja meg a vizsgálni kívánt felhasználó felhasználónevét (az a felhasználó, aki törölte az elemeket). A Tevékenységek **mezőben** válassza a **Törölt** üzenetek mappát, illetve az Üzenetek átkerülése a **Törölt elemek mappába elemet.**

4. Kattintson a **Keresés gombra.**

Az eredmények között jelöljön ki egy naplórekordot. A részleteket tartalmazó panelen kattintson a További **információ elemre.** A Törölt elemek mezőben további információk jelennek meg a törölt elemről (például a tárgysorról és az elem törlés utáni **helyéről).** A **ClientInfoString** tulajdonság meg fog mutatni, hogy a törlés Outlook, Webes Outlook (korábbi nevén Outlook Web App) vagy más eszközön történt-e.

További információ: Annak megállapítása, hogy ki állíthatja be az e-mail-továbbítást [egy postaládában.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)

**Megjegyzés:** A napló funkcióval nem lehet lekérni a törölt elemeket. A törölt üzenetek visszakeresését Webes Outlook [a Törölt](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)elemek helyreállítása a Outlook Web App.
