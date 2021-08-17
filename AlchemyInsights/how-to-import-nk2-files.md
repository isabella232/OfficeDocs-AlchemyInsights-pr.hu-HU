---
title: how-to-import-nk2-files
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: f2b034926ec165b819119b5c4e060f10022d6017ec5dba8794d18ee3e96c709a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54043208"
---
# <a name="how-to-import-nk2-files"></a>.nk2 fájlok importálása 

Az Microsoft Outlook 2013, Outlook 2016, Outlook 2019 vagy Microsoft 365-höz készült Outlook első elindítani a beceneve gyorsítótárát (amely *a* profilnév .nk2 fájlban van tárolva) az alapértelmezett üzenettárban lévő rejtett üzenetbe importálja.

Ha .nk2 fájlokat Outlook 2013-ba, Outlook 2016-be, Outlook 2019-be vagy Microsoft 365-höz készült Outlook-be importálni, győződjön meg arról, hogy a .nk2 fájl a következő mappában található: %appdata%\Microsoft\Outlook

**Megjegyzés:** A .nk2 fájlnak a jelenlegi 2013-as vagy 2013-as Outlook vagy Outlook 2016 kell lennie. A profilnév alapértelmezés szerint "nincs Outlook". A profilnév ellenőrzéshez kövesse az alábbi lépéseket: 
1. Kattintson a **Start** menü **Vezérlőpult** parancsára.
2. Kattintson duplán a Levelek **elemre.**
3. A Levelezési beállítások párbeszédpanelen válassza a **Profilok megjelenítése lehetőséget.**
4. Válassza a **Start** > **Futtatás** parancsot.
5. A Megnyitás **mezőbe írja** be az *outlook.exe /importnk2 parancsot,* majd válassza az **OK gombot.** 

A .nk2 fájl importálása után a fájl tartalma egyesül a postaládában tárolt becenév-gyorsítótárba.

**Megjegyzés:** A .nk2 kiterjesztést .old kiterjesztésűre nevezi át a rendszer, amikor legközelebb elindítja a Outlook 2013, Outlook 2016, Outlook 2019 vagy Microsoft 365-höz készült Outlook. Ha újra importálni szeretné a .nk2 fájlt, először távolítsa el a .old fájlnévkiterjesztést.

További információ: Az automatikus kiegészítési lista importálása vagy [másolása másik számítógépre.](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%)