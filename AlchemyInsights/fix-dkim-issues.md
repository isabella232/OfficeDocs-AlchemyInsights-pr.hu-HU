---
title: A DKIM beállítási hibáinak elhárítása
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744952"
---
# <a name="fix-dkim-setup-issues"></a>A DKIM beállítási hibáinak elhárítása

Ha problémákat tapasztal az egyéni tartomány DKIM engedélyezésével kapcsolatban, kövesse az alábbi lépéseket:

- A DKIM telepítési hibáinak többsége helytelen DNS-rekordokkal kapcsolatos. Ellenőrizze, hogy helyesen van-e formázva a DKIM CNAME rekordja (**nem** egy TXT rekord). További információt ebben a [témakörben](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)talál.

- Miután létrehozta vagy frissítette a DKIM DNS-rekordjait a tartományához tartozó DNS-szolgáltatónál (általában a tartományregisztráló), várja meg, amíg a DNS-rekordok propagálásra kerülnek.

- Ha nem tudja létrehozni a DKIM DNS-rekordjait a felügyeleti központban, lecserélheti az \<CustomDomain\> Egyéni tartományát (például contoso.com), és futtathatja ezt a parancsot az [Exchange Online PowerShellben](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
