---
title: DKIM beállítása egyéni tartományokkal
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/22/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: bb19f0672a21ea8b99c433ad83db4d89536c9a1705245fd2a683471170ab51ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994817"
---
# <a name="set-up-dkim-with-custom-domains"></a>DKIM beállítása egyéni tartományokkal

A DNS-ben minden egyes egyéni tartományhoz két CNAME rekordot kell közzétennie. Ehhez használja a következő formátumot:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> **A DomainGUID** az egyéni **tartományhoz** (például contoso-com az egyéni tartományhoz) a .mail.protection.outlook.com egyéni MX rekordban bal **oldali contoso.com).** **A InitialDomain** az a tartomány, amely a Office 365 (például a **contoso.onmicrosoft.com)** contoso.onmicrosoft.com.

A DNS-rekordokról a [DNS-rekordok](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)létrehozása bármely DNS-szolgáltatónál című Office 365.