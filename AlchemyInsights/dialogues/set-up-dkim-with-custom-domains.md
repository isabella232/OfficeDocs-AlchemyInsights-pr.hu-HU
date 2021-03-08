---
title: A DKIM beállítása egyéni tartományokkal
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
ms.openlocfilehash: c448956f0dad0738f4de7507ec4686c738a90a55
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524272"
---
# <a name="set-up-dkim-with-custom-domains"></a>A DKIM beállítása egyéni tartományokkal

A DNS-ben minden egyes egyéni tartományhoz két CNAME rekordot kell közzétennie. Ehhez használja az alábbi formátumot:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> **A DomainGUID** az egyéni tartomány testre szabott MX rekordja **.mail.protection.outlook.com** szövege (például a tartománynév contoso-com **contoso.com).** **A InitialDomain** az a tartomány, amit az Office 365-re való feliratkozáskor **használt (például** contoso.onmicrosoft.com).

A DNS-rekordokról további információt a DNS-rekordok létrehozása bármely [DNS-szolgáltatónál az Office 365-nek](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)című cikk tartalmaz.