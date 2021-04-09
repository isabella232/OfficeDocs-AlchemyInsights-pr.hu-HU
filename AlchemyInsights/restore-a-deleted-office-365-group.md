---
title: Törölt Microsoft 365-csoport visszaállítása
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
ms.openlocfilehash: b72b7c93ce9fe1b90d1608811b0eeabc8aec1363
ms.sourcegitcommit: a5edaaefdc56f8d5c8220a335f4e8228e2de4ee0
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/08/2021
ms.locfileid: "51645133"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Törölt Microsoft 365-csoport visszaállítása

A törölt Microsoft 365-csoportokat és Microsoft Teamseket a törléstől számított 30 napon belül visszaállíthatja.

1. Lépjen a [Microsoft 365](https://aka.ms/RestoreDeletedGroup) Felügyeleti központba, és jelentkezzen be a törölt csoportok és csapatok listájába.

    **Megjegyzés:** Jelentkezzen be a bérlői rendszergazdai vagy a csoport-rendszergazdai szerepkörhöz hozzárendelt fiókkal.

1. Jelölje ki a visszaállítani kívánt törölt Microsoft 365-csoportot/Teamst, és kattintson a **csoport visszaállítása elemre.**

    Ha a csoport nem állítható vissza ütköző SMTP-cím miatt, az alábbi paranccsal keresse meg az ütközést okozó objektumot, és távolítsa el az SMTP-címet:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Megjegyzés:** Bizonyos esetekben akár 24 óra is elehet, amíg a csoport és az összes adata visszaállítható.

    További információért, illetve a csoportok PowerShell használatával való visszaállításáról a Törölt [Microsoft 365-csoport](https://go.microsoft.com/fwlink/?linkid=867802)visszaállítása.