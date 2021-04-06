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
ms.openlocfilehash: caa2c8987eecb89bac3469bf9471847858cab0ba
ms.sourcegitcommit: ec99a3a2e1e6a13d9a829d65ad1692a607dc3a17
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/06/2021
ms.locfileid: "51597445"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Törölt Microsoft 365-csoport visszaállítása

A törölt Microsoft 365-csoportokat és Microsoft Teamseket a törléstől számított 30 napon belül visszaállíthatja.

1. Lépjen a [Microsoft 365](https://aka.ms/RestoreDeletedGroup) Felügyeleti központba a bejelentkezéshez, és sorolja fel a törölt csoportokat és csoportokat.

    **Megjegyzés:** Jelentkezzen be a bérlői rendszergazdai vagy a csoport-rendszergazdai szerepkörhöz hozzárendelt fiókkal.

1. Jelölje ki a visszaállítani kívánt törölt Microsoft 365-csoportot/Teamst, és kattintson a **csoport visszaállítása elemre.**

    Ha a csoport nem állítható vissza ütköző SMTP-cím miatt, az alábbi paranccsal keresse meg az ütközést okozó objektumot, és távolítsa el az SMTP-címet:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Megjegyzés:** Bizonyos esetekben akár 24 óra is elehet, amíg a csoport és az összes adata visszaállítható.

    További információért, illetve a csoportok PowerShell használatával való visszaállításáról a Törölt [Microsoft 365-csoport](https://go.microsoft.com/fwlink/?linkid=867802)visszaállítása.