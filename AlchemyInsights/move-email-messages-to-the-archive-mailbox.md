---
title: E-mail-üzenetek áthelyezése az archív postaládába
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
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799782"
---
# <a name="move-email-to-the-archive-mailbox"></a>E-mailek áthelyezése az archív postaládába

Ha azt szeretné, hogy az alábbi beállítások automatikus ellenőrzését végezze el, válassza a vissza < gombot a lap tetején, és írja be annak a felhasználónak az e-mail-címét, aki problémákat tapasztal az e-mailek archív postaládájába való áthelyezésével kapcsolatban.

1. Ellenőrizze, hogy engedélyezve van-e egy **archív postaláda** . Ha nem, akkor a [jelen cikkben](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) található lépéseket követve engedélyezze az archív postaládát.

2. Ha automatikusan szeretné archiválni az üzeneteket az archív postaládába, az **Áthelyezés az archiválási** eljárásra beállításnál a **teljes postaláda (alapértelmezett) címkére kell alkalmazni**az adatmegőrzési címkét. Az alábbi lépésekkel hozhatja létre a címkét: [Archívum alapértelmezett címke](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Ezután adja hozzá az **archív** címkét az adatmegőrzési házirendhez. Az Exchange felügyeleti központban válassza az **adatmegőrzési házirendek** > az **Áthelyezés az archívumba címkét** a házirend > **Mentés**elemre.

4. Most [rendelje az adatmegőrzési házirendet](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) az adott felhasználó postaládájához. Ugyanezt a házirendet alkalmazza mind az **elsődleges** , mind az **archív** postaládára.

Előfordulhat, hogy a felügyelt mappa Segédének (MFA) kell kikényszeríteni, hogy fusson, és az új beállításokat alkalmazza a felhasználó postaládájába. Futtassa az alábbi parancsot, miközben az [EXO powershellhez csatlakozik](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) , és egy adott postaládához szeretné elindítani a felügyelt mappa Segédet:
  
Start – ManagedFolderAssistant – identitás <name of the mailbox>

Az archiválási házirend beállításáról további információt a [postaládák archiválási és törlési házirendjének beállítása](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)című témakörben talál.
  