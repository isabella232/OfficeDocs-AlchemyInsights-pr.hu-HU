---
title: E-mailek áthelyezése az archív postaládába
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 5592bc7d4566e3498c33bbf9488db7f46ec58842
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822164"
---
# <a name="move-email-to-the-archive-mailbox"></a>E-mailek áthelyezése az archív postaládába

1. Ellenőrizze, hogy az **archív postaláda** engedélyezve van-e. Ha nem, akkor az ebben a [cikkben](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) leírt lépésekkel engedélyezheti az archív postaládát.

2. Ha automatikusan szeretné archiválni az üzeneteket az archív postaládába, az **Áthelyezés az archiválandó** műveletre beállított adatmegőrzési címkét a **teljes postafiók (alapértelmezett) címke automatikus alkalmazására**kell állítani. Használja a lépéseket ide, hogy megteremtse a tag: [Archívum default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Ezután adja hozzá az **archív** címkét az adatmegőrzési szabályhoz. Az Exchange felügyeleti központban válassza az **adatmegőrzési szabályok** > az **Áthelyezés az archív címkéhez** parancsot a > **Mentés**házirendbe.

4. [Rendelje hozzá az adatmegőrzési szabályt](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) az adott felhasználó postaládájához. Ugyanez a házirend vonatkozik az **elsődleges** és az **archív** postaládára is.

Szükség lehet a kezelt mappák segédjének (MFA) futtatására, és az új beállításoknak a felhasználó postaládájára történő alkalmazására. Futtassa a következő parancsot, miközben [csatlakozik az EXO PowerShell-hoz](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) a kezelt mappa segéd indításához egy adott postafiókhoz:
  
Start-ManagedFolderAssistant-identitás<name of the mailbox>

Az archiválási házirendek beállításával kapcsolatos további tudnivalókért tanulmányozza a [postaládák archiválási és törlési házirendjének beállítása](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)című témakört.
  