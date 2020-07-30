---
title: E-mailek áthelyezése az Archív postaládába
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 9af8a4d3ce72fd901ff2f3a1aae0654c7213dd7e
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522773"
---
# <a name="move-email-to-the-archive-mailbox"></a>E-mailek áthelyezése az archív postaládába

Ha azt szeretné, hogy automatikusan ellenőrizze az alább említett beállításokat, válassza a vissza gombot < - az oldal tetején, majd adja meg annak a felhasználónak az e-mail címét, akinek problémái vannak az e-mailek áthelyezésével az archív postaládájába.

1. Ellenőrizze, hogy engedélyezve **van-e az archív postaláda.** Ha nem, a [cikkben](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) ismertetett lépésekkel engedélyezze az archív postaládát.

2. Ha az üzeneteket automatikusan archiválni szeretné az archív postaládába, **be** kell állítania, hogy az automatikusan alkalmazza a **teljes postaláda -ra (alapértelmezett) címkét.** Az itt leírt lépésekkel hozhatja létre a címkét: [Archiválás i. címke](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Ezután adja hozzá az **Archív** címkét az adatmegőrzési házirendhez. Az Exchange Felügyeleti központban válassza az **Adatmegőrzési házirendek** lehetőséget, > adja hozzá az **Áthelyezés az archívumba címkét** a Mentés > **házirendhez.**

4. Most [rendelje hozzá az adatmegőrzési szabályt](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) az adott felhasználó postaládájához. Ugyanez a házirend lesz alkalmazva mind az **Elsődleges,** mind az **Archív** postaládára.

Szükség lehet arra, hogy a felügyelt mappasegédet (MFA) a felhasználó postaládájára kényszerítse és alkalmazza az új beállításokra. Futtassa a következő parancsot, miközben [az EXO PowerShellhez csatlakozik](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) egy adott postaláda felügyelt mappasegédének elindításához:
  
Start-ManagedFolderAssistant -Identitás<name of the mailbox>

Az archiválási házirend beállításáról a [postaládák archiválási és törlési házirendjének beállítása](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)című témakörben talál további információt.
  