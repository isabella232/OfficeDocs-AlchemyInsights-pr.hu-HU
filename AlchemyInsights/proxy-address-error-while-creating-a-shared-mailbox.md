---
title: Proxycímhiba megosztott postaláda létrehozásakor
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568292"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Proxycímhiba postaláda vagy más levelezési objektum létrehozása közben

Ha megpróbál létrehozni egy e-mail-kompatibilis objektumot (postaláda, megosztott postaláda stb.), és "A proxycím "SMTP:alias@domain.com" már használatban van..." hibaüzenet jelenik meg, akkor a választott e-mail-címet már a szervezet egy másik e-mail-képes objektuma hozza létre.
  
Meg kell találnia az e-mail-címet tartalmazó felhasználót, csoportot, megosztott postaládát vagy nyilvános mappát, és törölnie kell azt, vagy módosítania kell az e-mail-címét. Ezután létrehozhat egy új, e-mail-címmel rendelkező objektumot a felszabadított e-mail címmel. A kereséshez használja a Keresés lapot a kezdőlapon. A következő Exchange Online PowerShell-paranccsal is megkeresheti:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Ha nem szeretné törölni a meglévő e-mail-címet, válasszon egy új e-mail-címet a létrehozott új objektumhoz.
  