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
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717564"
---
# <a name="fix-dkim-setup-issues"></a>A DKIM beállításával kapcsolatos problémák megoldása

Ha problémákat tapasztal a DKIM egyéni tartományhoz való engedélyezésével kapcsolatban, kövesse az alábbi lépéseket:

- A DKIM legtöbb beállítási problémája helytelen DNS-rekordokhoz kapcsolódik. Ellenőrizze, hogy a DKIM CNAME rekord **(nem** TXT rekord) megfelelően van-e formázva. További információt ebben a [témakörben talál.](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)

- Miután létrehozta vagy frissítette a DKIM DNS-rekordjait a tartománydns-szolgáltatónál (általában a tartományregisztrálónál), várja meg, amíg a DNS-rekordok propagálnak.

- Ha nem tudja létrehozni a DKIM DNS-rekordokat a \<felügyeleti\> központban, lecserélheti az Egyéni tartományt az egyéni tartományra (például contoso.com), és futtathatja ezt a parancsot az [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)ben: `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.
