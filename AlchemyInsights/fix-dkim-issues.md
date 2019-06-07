---
title: DKIM telepítésével kapcsolatos problémák megoldása
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765131"
---
# <a name="fix-dkim-setup-issues"></a>DKIM telepítésével kapcsolatos problémák megoldása

Ha az egyéni tartomány DKIM engedélyezése problémákat tapasztal, használja az alábbi lépéseket:

- A legtöbb DKIM telepítésével kapcsolatos problémák kapcsolatos helytelen DNS-rekordokat. Ellenőrizze a DKIM CNAME rekordot (**nem** TXT rekord) megfelelően van formázva. További tudnivalókért tanulmányozza a [témakör](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- Miután létrehozása vagy frissítése a DKIM DNS-rekordokat a DNS-szolgáltatás a tartományba (általában a tartomány hivatalvezető), várja a DNS-rekordok terjesztése.

- Ha nem lehet létrehozni a DKIM DNS bejegyzések az admin center, csere \<CustomDomain\> az egyéni tartomány (például contoso.com) és futtatni ezt a parancsot az [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.
