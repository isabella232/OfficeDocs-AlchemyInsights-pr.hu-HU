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
ms.openlocfilehash: 7c15d5db5445fbe4c3ec22878f180f48d2da4f90369f2e6f223916646eb19c12
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54062910"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Proxycímhiba postaláda vagy más levelezési objektum létrehozásakor

Ha egy e-mail-címmel rendelkező objektum (postaláda, megosztott postaláda stb.) létrehozása után "A "SMTP:alias@domain.com" proxycím már használatban van..." hibaüzenet jelenik meg, akkor a választott e-mail-címet már a szervezet egy másik e-mail-címmel rendelkező objektuma hozza létre.
  
Meg kell találnia az e-mail-címet tartalmazó felhasználót, csoportot, megosztott postaládát vagy nyilvános mappát, és törölnie kell azt, vagy módosítania kell az e-mail-címét. Ezután létrehozhat egy új, e-mail címmel rendelkező, e-mail címmel rendelkező objektumot. A kereséshez használja a Keresés lapot a Kezdőlap lapon. A PowerShell Exchange Online az alábbi parancsokkal is megkeresheti:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Ha nem szeretné törölni a meglévő e-mail-címet, válasszon egy új e-mail-címet a létrehozni kívánt új objektumhoz.
  