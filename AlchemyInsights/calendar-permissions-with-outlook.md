---
title: Naptár engedélyei
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862093"
---
# <a name="calendar-permissions"></a>Naptár engedélyei

A felhasználók módosíthatják saját naptárengedélyeiket a Webes Outlookkal vagy más ügyfelekkel, de rendszergazdaként előfordulhat, hogy a vizsgálatot is meg kell vizsgálnia.  
Az Exchange PowerShell-parancsmaggal megmutatja a felhasználó naptárának engedélyét:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

További információkért lásd a következő témakört:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Mailboxfolder hozzáadása](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

A naptárengedélyek a naptárak megosztásában használatosak, és további információkat kaphat az Outlook-naptármegosztásról, lásd az alábbi cikkeket:

- [Outlook-naptár megosztása másokkal](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Naptár megosztása a Webes Outlookban](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

A Naptár engedély hibaelhárításához használja a [Támogatási és helyreállítási segéd](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) eszközt.