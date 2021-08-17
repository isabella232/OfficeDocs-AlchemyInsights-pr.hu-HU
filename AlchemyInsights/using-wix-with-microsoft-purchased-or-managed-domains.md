---
title: Wix-webhely használata megvásárolt vagy felügyelt Microsoft-tartományokkal
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5855"
- "9003096"
ms.openlocfilehash: dd0f8beb8f1871c2c43ac14a7f6d1cce79386fcc353bb2a690ba184904ca5857
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083736"
---
# <a name="using-a-wix-website-with-microsoft-purchased-or-managed-domains"></a>Wix-webhely használata megvásárolt vagy felügyelt Microsoft-tartományokkal

A Wix-webhely Microsoft által vásárolt vagy felügyelt tartománnyal való használatával kapcsolatban A DNS-rekordok frissítése, hogy a webhely a jelenlegi tárhelyszolgáltatónál maradjon című cikk [nyújt tájékoztatást.](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)

Részletes információkért lásd: 

- A "Connecting a Domain to Wix Using the Pointing Method" (Tartomány csatlakoztatása Wix-kiszolgálóhoz a pointing metódussal) című cikk azt javasolja, hogy a fenti hivatkozásnak megfelelő DNS-rekordokat adjon hozzá ahelyett, hogy a névkiszolgálókat módosítja a Microsoft 365.

- Ha a névkiszolgálók Wixre való átváltását választja, a Microsoft Wix rendszerében létre kell hoznia a DNS-rekordokat. További információt a [DNS-rekordok létrehozása a Microsoft Wix rendszerében című cikk tartalmaz.](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix)

- Ha tartományát a Microsofttól vásárolta, a névkiszolgálók nem módosíthatók. Ha módosítania kell a névkiszolgálókat, a Microsoft által vásárolt tartományt 60 nap múlva át kell helyezni egy másik szolgáltatóhoz. További információt a Tartomány [átvitele a Microsofttól egy másik szolgáltatóhoz .](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)
