---
title: 1336 RecoverableItems mappa megtelt
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 4f0cba480fcc05114abd8f370b84e9a37e5f2804
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510754"
---
# <a name="the-recoverable-items-folder-is-full"></a>A Helyreállítható elemek mappa megtelt

Exchange Online-postaládák esetén a Helyreállítható elemek mappa alapértelmezett tárolási korlátja 30 GB. A Helyreállítható elemek mappa tárolási korlátja automatikusan 100 GB-ra nő, ha a postaláda peres eljárás miatti tartásba, elektronikus adatfeltárási visszatartásba kerül, vagy adatmegőrzési házirendhez van rendelve.

Amikor a Helyreállítható elemek mappa eléri a tárolási korlátot, a postaláda funkciója a következő módokon változik:

- A felhasználó nem törölhet elemeket a postaládából.

- A Felügyelt mappasegéd nem tudja törölni az elemeket az adatmegőrzési címke vagy a kezelt mappa beállításai alapján.

- Az on-item recovery engedélyezve van vagy várakoztatott postaládák esetében az írásra másolási oldal védelmi folyamata nem tudja karbantartani a felhasználó által szerkesztett elemek verzióit.

- Azon postaládák esetében, amelyeknél engedélyezve van a postaláda naplózása, a Helyreállítható elemek mappa Naplózás almappájába nem lehet postaláda-naplóbejegyzéseket menteni.

A nem várakoztatott postaládák esetén a rendszergazdák az `Search-Mailbox -SearchDumpsterOnly -DeleteContent` Exchange Online PowerShell parancsával törölhetik a Helyreállítható elemek mappában lévő elemeket. További tudnivalókat a következő témakörökben talál:

- [Üzenetek keresése és törlése](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Keresés-postaláda](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

A várakoztatott postaládák esetében a rendszergazdáknak el kell távolítaniuk a visszatartást, mielőtt törölhetik az elemeket a Helyreállítható elemek mappából. További információt az [Elemek törlése a felhőalapú postaládák visszatartott helyreállítható elemek mappájában című témakörben talál.](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)

A Helyreállítható elemek mappa megteltsíthetőj, a rendszergazdák növelhetik a visszatartott postaládák Helyreállítható elemek mappájának tárolási korlátját, és beállíthatnak egy postaláda-adatmegőrzési házirendet, amely a Helyreállítható elemek mappából a felhasználó archív postaládájába helyezi át az elemeket. Lásd: [A visszatartott postaládák helyreállítható elemek kvótájának növelése.](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold)
