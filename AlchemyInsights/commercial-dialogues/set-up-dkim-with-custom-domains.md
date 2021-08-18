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
ms.openlocfilehash: cb1f621dffc88464c339b55998efb5440cfd775c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332309"
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
**Megjegyzés:** **A DomainGUID** a **.mail.protection.outlook.com** egyéni tartomány testre szabott MX rekordja (például contoso-com a tartománynévben) **bal contoso.com).** **A InitialDomain** az a tartomány, amely a Office 365 (például a **contoso.onmicrosoft.com)** contoso.onmicrosoft.com.

A DNS-rekordokról további információt a [DNS-rekordok](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)létrehozása bármely DNS-szolgáltatónál a Office 365.