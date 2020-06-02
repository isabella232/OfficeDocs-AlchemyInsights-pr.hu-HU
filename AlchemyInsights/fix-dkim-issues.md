---
title: A DKIM beállításával kapcsolatos problémák megoldása
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506776"
---
# <a name="fix-dkim-setup-issues"></a>A DKIM beállításával kapcsolatos problémák megoldása

Ha problémákat tapasztal a DKIM egyéni tartományhoz való engedélyezésével kapcsolatban, kövesse az alábbi lépéseket:

- A DKIM legtöbb beállítási problémája helytelen DNS-rekordokhoz kapcsolódik. Ellenőrizze, hogy a DKIM CNAME rekord **(nem** TXT rekord) megfelelően van-e formázva. További információt ebben a [témakörben talál.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

- Miután létrehozta vagy frissítette a DKIM DNS-rekordjait a tartománydns-szolgáltatónál (általában a tartományregisztrálónál), várja meg, amíg a DNS-rekordok propagálnak.

- Ha nem tudja létrehozni a DKIM DNS-rekordokat a felügyeleti központban, lecserélheti \<CustomDomain\> az egyéni tartományra (például contoso.com), és futtathatja ezt a parancsot az [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)ben: `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
