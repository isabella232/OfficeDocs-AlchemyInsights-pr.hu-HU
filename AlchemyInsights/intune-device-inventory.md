---
title: Intune Eszközkészlet
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 00ee4f1d7130c239272e28ee8e051a18e6e0baf13040d2a892866be5900adfaf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54014074"
---
# <a name="intune-device-inventory"></a>Intune Eszközkészlet

Az Eszközök blade eszközenként betekintést nyújt a rendszergazda számára az Intune kezelés alatt álló eszközeibe. A megjelenő információk közé tartozik a következő: Hardver, Talált alkalmazások, Eszköz megfelelőségi állapota és Eszközkonfigurációs állapot.

A hardveres és a talált alkalmazások készletadatokat egy hét napos ciklusban gyűjti össze. A jelentett alkalmazások és hardverelemek eltérhetnek az eszköz operációs rendszerétől, illetve attól függően, hogy az eszköz személyes vagy vállalati tulajdonú-e.

További információt az Eszközadatok megtekintése [az Intune-ban.](https://docs.microsoft.com/intune/device-inventory)

**GYIK**

K: Nem kapom meg az Intune által regisztrált összes alkalmazás teljes készletlistát az Windows eszközön. miért ne?

K: Jelenleg csak a vállalati eszközként azonosított számítógépekhez Windows 10 modern appok vannak felsorolva. Az Intune nem gyűjt adatokat az ilyen eszközökön telepített Win32-alkalmazásokról.

K: Miért nem gyűjtjük a telefonszámokat az összes eszközről?

A: Az Intune-ban a vállalati eszközökként kategorizált telefonokat a rendszer nem azonosítja a teljes telefonszámmal, ha például egy mobileszköz készletjelentését futtatja. A saját eszközével hozó telefonszámokat mindig részben csillaggal (****) takarja el a rendszer, és csak az utolsó négy számjegyet mutatja.