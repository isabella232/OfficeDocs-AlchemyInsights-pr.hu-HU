---
title: Adatok helye
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655284"
---
# <a name="data-location"></a>Adatok helye

Megtekintheti a bérlő helyét a felügyeleti központban, vagy az Exchange Online-hoz a PowerShellen keresztül való csatlakozással.


**Felügyeleti központ:**
1. Jelentkezzen be a [felügyeleti központba](https://admin.microsoft.com/Adminportal/Home).
2. Válassza a **Beállítások** > **szervezet profil lehetőséget.**
3. Az **Adatok helye csoportban**válassza **a Részletek megtekintése**lehetőséget.


**Powershell:**
1. Csatlakozzon az Exchange Online-hoz a Windows PowerShell használatával.
2. A [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) parancsmag végrehajtása a bérlő tulajdonságainak listájának megjelenítéséhez. 
3. Nézd meg a OrganizationId tulajdonát.

Ha rendelkezik az EXO és az SPO adathelyével, meghatározhatja az adatok helyét más szolgáltatásokhoz, amelyeket [az Adatok helye](https://products.office.com/where-is-your-data-located)helye alapján használhat.