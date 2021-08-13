---
title: 1336 RecoverableItems mappa megtelt
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
ms.openlocfilehash: 5c8d53ceabf2428f3d6d765040f1b789b6bbeda04a22dd7fde0d2d728fd17d93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061758"
---
# <a name="the-recoverable-items-folder-is-full"></a>Megtelt a Helyreállítható elemek mappa

A Exchange Online esetén a Helyreállítható elemek mappa alapértelmezett tárterületkorlátja 30 GB. A Helyreállítható elemek mappa tárterületkorlátja automatikusan 100 GB-ra nő, ha a postaláda jogi visszatartásra, adatfeltárási visszatartásra kerül, vagy ha adatmegőrzési házirendhez van rendelve.

Amikor a Helyreállítható elemek mappa eléri a tárterületkorlátot, a postaláda működését az alábbi módokon érinti:

- A felhasználó nem tud elemeket törölni a postaládából.

- A Felügyeltmappa-segéd nem tud elemeket törölni az adatmegőrzési címke vagy a felügyelt mappa beállításai alapján.

- Az olyan postaládák esetén, amelyekben engedélyezve van az egyelemű helyreállítás, vagy amelyekre a rendszer vissza szeretné őket helyezni, az írási másolásos lapvédelmi eljárás nem tudja karbantartani a felhasználó által szerkesztett elemek verzióit.

- Azok a postaládák, amelyekben engedélyezve van a postaláda-naplózás, a Postaládák naplóbejegyzései nem menthetők a Helyreállítható elemek mappa Naplók almappába.

A nem visszatartott postaládákban a rendszergazdák a PowerShell Exchange Online paranccsal törölhetik a Helyreállítható elemek mappában `Search-Mailbox -SearchDumpsterOnly -DeleteContent` lévő elemeket. További tudnivalókat a következő témakörökben talál:

- [Üzenetek keresése és törlése](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

A visszatartott postaládákban a rendszergazdának el kell távolítania a törlési parancsot ahhoz, hogy töröljön elemeket a Helyreállítható elemek mappából. További információ: [Törlés](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)a felhőalapú postaládák Helyreállítható elemek mappájában.

Ha meg szeretné akadályozni, hogy a Helyreállítható elemek mappa teljesen megteljön, a rendszergazdák növelhetik a visszatartás alatt lévő postaládák Helyreállítható elemek mappájának tárterületkorlátját, és állíthatnak be egy olyan postaláda-adatmegőrzési házirendet, amely áthelyezi az elemeket a Helyreállítható elemek mappából a felhasználó archív postaládájába. Lásd: A tartható postaládák Helyreállítható [elemek kvótájának növelése.](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold)
