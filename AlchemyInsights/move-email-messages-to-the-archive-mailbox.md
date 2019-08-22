---
title: E-mailek áthelyezése az archív postaláda
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
ms.openlocfilehash: ce52df446fc4c23c06476e8836ade6a6810d158f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36549005"
---
# <a name="move-email-to-the-archive-mailbox"></a>E-mail áthelyezése az archív postaláda

1. Győződjön meg arról, hogy a **postaláda archiválása** engedélyezve van. Ha nem, az archív postaláda engedélyezése [Ebben](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) a cikkben leírtakat.

2. Archiválása az archív postaláda üzeneteket automatikusan, az **Ugrás archiválása** művelettel adatmegőrzési címke **automatikusan**alkalmazandó teljes postafiók (alapértelmezés) címkével kell állítani. Kövesse a lépéseket Itt a címke létrehozása: [Archív alapértelmezett címkét](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).

3. Ezután adja hozzá az **Archív** címke az adatmegőrzési szabály. Válassza ki az Exchange felügyeleti központ **Adatmegőrzési** > hozzá a **címke archívum áthelyezése** a házirend > **menteni**.

4. Most [a megőrzési házirendet](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) az adott felhasználó postaládájához. Ugyanaz a házirend az **elsődleges** és az **Archív** postaláda vonatkozik.

A kezelt mappa Segéd (MFA) és az új beállítások alkalmazása a felhasználó postaládájában, hogy szükség lehet. Futtassa a következő parancsot közben [csatlakoztatva EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) indítása a kezelt Mappakezelő egy adott postaláda:
  
Start-ManagedFolderAssistant-azonosító<name of the mailbox>

Archiválási házirend beállításával kapcsolatos további tudnivalókért lásd [az archív és törlési házirend postafiókok beállítása](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  