---
title: Műveletnaplók törlése üzenet események azonosítása
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 89877331d328d798177fab3150d5219c5b484a70
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35383135"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Naplók a törölt e-mailek

Január 2019 kezdődően a Microsoft van bekapcsolása alapértelmezés szerint a postafiók naplóvizsgálat. Ellenkező esetben üzenet események törlése egy adott felhasználó áttekintéséhez kell manuálisan engedélyezi a törlési műveletek naplózását. Ha a postaláda naplózása naplózási már engedélyezve van a szervezet számára, vagy az adott felhasználó, kövesse az alábbi lépéseket.

1. Jelentkezzen be az [Office 365 biztonsági & kompatibilitási központ](https://protection.office.com/)

2. Kattintson a **Keresés és a vizsgálat** , és válassza a **Könyvvizsgálati napló Search**.

3. Jelöljük ki a dátumot a **Kezdő dátum** és **Záró dátum** mezőket. Adja meg a felhasználó (Törölt elemek a felhasználó) vizsgálja meg a használni kívánt felhasználónév. A **tevékenységek** mezőben jelölje ki a **Törölt elemek mappából törölt üzenetek** és a **Moved üzenetek a törölt elemek mappába**.

4. Kattintson a **Keresés**gombra.

Az eredmények a válassza ki a tételt generál. Kattintson a részletek úszó **További információ**. További információt a törölt elem (például a tárgy és a hely törlésekor a program a cikk) a **AffectedItems** mezőben jelenik meg. A **ClientInfoString** tulajdonság fogja mutatni, ha a törlés történt, az Outlook, az Outlook a weben (korábbi nevén az Outlook Web App), vagy bármely más eszköz.

További információért lásd: [aki postaládához továbbítása e-mail beállítás meghatározása](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).

**Megjegyzés**: nem lehet beolvasni a törölt elemek a könyvvizsgálati napló szolgáltatásával. Beolvasni a törölt üzeneteket az Outlook programban a weben, lásd: [Törölt elemek az Outlook Web App helyreállítása](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
