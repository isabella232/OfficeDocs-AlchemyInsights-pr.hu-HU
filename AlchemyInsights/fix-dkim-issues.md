---
title: A DKIM beállítási problémáinak elhárítása
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
ms.openlocfilehash: 5a613321ed79e657350ec4d19b1f07ac0a091b227a8268c793a10edd9990d41f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945933"
---
# <a name="fix-dkim-setup-issues"></a>A DKIM beállítási problémáinak elhárítása

Ha problémákat tapasztal a DKIM egyéni tartományhoz való engedélyezése során, kövesse az alábbi lépéseket:

- A DKIM beállításával kapcsolatos legtöbb probléma helytelen DNS-rekordokhoz kapcsolódik. Ellenőrizze, hogy **a** DKIM CNAME rekord (nem TXT rekord) megfelelően van-e formázva. További információt ebben a [témakörben található.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

- Miután a DKIM DNS-rekordokat a tartomány DNS-szolgáltatójánál (tipikusan a tartományregisztrálónál) létrehozott vagy frissíti, várja meg, amíg meg nem propagálják a DNS-rekordokat.

- Ha nem tudja létrehozni a DKIM DNS-rekordokat a felügyeleti központban, lecserélheti az egyéni tartományát (például contoso.com), és futtathatja ezt a parancsot a \<CustomDomain\> [Exchange Online PowerShellben:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
