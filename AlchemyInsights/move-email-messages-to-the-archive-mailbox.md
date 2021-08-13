---
title: E-mailek áthelyezése az archív postaládába
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
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 7e72766f441e210a81fcfd6c07b1801f6c0474afb02a70edf2ad8dbb571f3d2a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974959"
---
# <a name="move-email-to-the-archive-mailbox"></a>E-mailek áthelyezése az archív postaládába

Ha azt szeretné, hogy automatikusan ellenőrizjük az alább említett beállításokat, válassza a vissza gombot < - a lap tetején, majd adja meg annak a felhasználónak az e-mail-címét, aki problémákat tapasztal az e-mailek archív postaládába való áthelyezésével kapcsolatban.

1. Ellenőrizze, hogy engedélyezve **van-e** az archív postaláda. Ha nem, a [](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) cikkben található lépéseket követve engedélyezze az archív postaládát.

2. Az üzenetek archiválásához az archív  postaládába való automatikus archiváláshoz az Áthelyezés archívumba művelethez beállított adatmegőrzési címkét automatikusan alkalmazni kell a teljes **postaláda (alapértelmezett) címkére.** A címke létrehozásához kövesse az alábbi lépéseket: [Alapértelmezett címke archiválása.](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)

3. Ezután adja hozzá az **Archiválás** címkét az adatmegőrzési házirendhez. A Exchange Felügyeleti központban válassza az Adatmegőrzési házirendek **lehetőséget,** > adja hozzá az Áthelyezés az archívumba címkét a házirendhez a > **gombra.** 

4. Most [rendelje hozzá az adatmegőrzési házirendet](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) az adott felhasználó postaládájához. A rendszer ugyanezt a házirendet alkalmazza az Elsődleges **és** az Archív **postaládára is.**

Előfordulhat, hogy futtatni kell a Felügyeltmappa-segédet (MFA), és alkalmaznia kell az új beállításokat a felhasználó postaládájára. Futtassa az alábbi parancsot, miközben csatlakozik [az EXO PowerShellhez,](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) és indítsa el a Felügyeltmappa-segédet egy adott postaládához:
  
Start-ManagedFolderAssistant -Identity <name of the mailbox>

Az archiválási házirendek beállításával kapcsolatos további információkért lásd: Archiválási és törlési házirend beállítása [postaládákhoz.](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)
  