---
title: Naptár engedélyei
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: cfee520e26587c0a649c08084853c31232d027f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748795"
---
# <a name="calendar-permissions"></a>Naptár engedélyei

A felhasználók megváltoztathatják a saját naptáruk engedélyeit a webes Outlookban vagy más ügyfélprogramokban, de rendszergazdaként is szükség lehet a vizsgálatra.  
Az Exchange PowerShell-parancsmaggal megjelenítheti a felhasználó naptárának engedélyét:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

További információk a következő témakörökben olvashatók:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Naptár-engedélyek használata a naptárak megosztásában: az Outlook naptárának megosztásáról további információt az alábbi cikkekben talál:

- [Outlook-naptár megosztása másokkal](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Naptár megosztása a webes Outlook vállalati verzióban](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

A naptár engedélyeinek elhárításához használhatja a [támogatási és helyreállítási segéd](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) eszközt.