---
title: Törölt csoport Microsoft 365 visszaállítása
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: 6262ca04335c355fb4de41a9e1d854b666f47e10321a843717d6eb951c46cafd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959028"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Törölt csoport Microsoft 365 visszaállítása

A törölt csoportokat Microsoft 365 30 Microsoft Teams belül visszaállíthatja.

1. Lépjen a [Microsoft 365 Felügyeleti központ](https://aka.ms/RestoreDeletedGroup) a törölt csoportok és csapatok listájába való bejelentkezéshez.

    **Megjegyzés:** Jelentkezzen be a bérlői rendszergazdai vagy a csoport-rendszergazdai szerepkörhöz hozzárendelt fiókkal.

1. Jelölje ki a visszaállítani Microsoft 365 törölt csoportokat Teams, és kattintson a csoport **visszaállítása elemre.**

    Ha a csoport nem állítható vissza ütköző SMTP-cím miatt, az alábbi paranccsal keresse meg az ütközést okozó objektumot, és távolítsa el az SMTP-címet:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Megjegyzés:** Bizonyos esetekben akár 24 óra is elehet, amíg a csoport és az összes adata visszaállítható.

    További információt, illetve a csoportok PowerShell használatával való visszaállításáról a Törölt csoportok visszaállítása Microsoft 365 [olvashat.](https://go.microsoft.com/fwlink/?linkid=867802)