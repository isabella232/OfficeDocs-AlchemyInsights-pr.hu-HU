---
title: a 1336 RecoverableItems mappája megtelt
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
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741269"
---
# <a name="the-recoverable-items-folder-is-full"></a>A helyreállítható elemek mappa megtelt

Az Exchange Online-postaládák esetében a helyreállítható elemek mappa alapértelmezett tárterülete 30 GB. A helyreállítható elemek mappa tárterülete automatikusan 100 GB-ra növekszik, ha a postaláda jogellenes tartásra, eDiscovery tartása vagy adatmegőrzési házirendhez van rendelve.

Ha a helyreállítható elemek mappa eléri a tárterületet, a postaláda működését az alábbi módokon érinti:

- A felhasználó nem tud elemeket törölni a postaládából.

- A felügyelt mappa Segéd nem tudja törölni az elemeket adatmegőrzési címke vagy a felügyelt mappa beállításai alapján.

- Az egyelemes helyreállítást engedélyező vagy felfüggesztett postaládák esetén a copy-on-Write lap védelmi folyamata nem tudja megőrizni a felhasználó által szerkesztett elemek verziószámát.

- Ha a postaláda-naplózás engedélyezve van, a postaláda-naplózási bejegyzéseket nem lehet menteni a helyreállítható elemek mappa naplózási almappájában.

A nem tartott postaládák esetében a rendszergazdák az `Search-Mailbox -SearchDumpsterOnly -DeleteContent` Exchange Online PowerShellben a parancs segítségével törölhetik az elemeket a helyreállítható elemek mappában. További tudnivalókat a következő témakörökben talál:

- [Üzenetek keresése és törlése](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Keresés a postaládában](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

A levezetett postaládák esetében a rendszergazdáknak el kell távolítaniuk a mentességet, mielőtt a helyreállítható elemek mappából törölt elemek. További tudnivalókat az [elemek törlése a felhőalapú postaládák visszanyerhető elemek mappájából lenyomva](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)című témakörben találhat.

Ha meg szeretné akadályozni, hogy a helyreállítható elemek mappa teljes mértékben megmaradjon, a rendszergazdák növelhetik a helyreállítható elemek mappa tárolási korlátját, és beállíthatja a postaláda-adatmegőrzési házirendet, amely áthelyezi az elemeket a helyreállítható elemek mappából a felhasználó archív postaládájába. Lásd: [a helyreállítható elemek visszanyerhető kvótájának növelése a letartott postaládákban](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
