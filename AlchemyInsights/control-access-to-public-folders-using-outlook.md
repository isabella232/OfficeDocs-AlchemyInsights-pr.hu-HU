---
title: A nyilvános mappákhoz való hozzáférés szabályozása az Outlook használatával
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 1386b97f804e63455094abf64b9d9e2541d57dafa36535813b0d7689e0ce2966
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54032560"
---
# <a name="control-access-to-public-folders-using-outlook"></a>A nyilvános mappákhoz való hozzáférés szabályozása az Outlook használatával

A nyilvános mappákhoz hozzáférő felhasználók szabályozásához az Outlook használatával:

1. A `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false` használata

$true: Nyilvános mappák elérésének engedélyezése a felhasználóknak az Outlookban  
$false: A nyilvános mappák elérésének megakadályozása az Outlookban. Ez az alapértelmezett érték.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Megjegyzés: Ez az eljárás csak a Windows rendszerű asztali Outlook kapcsolatokat szabályozhatja. A felhasználók továbbra is hozzáférhetnek a nyilvános mappákhoz az OWA vagy a Mac Outlook használatával.

További információért lásd: [Ellenőrzött kapcsolatok a nyilvános mappákkal az Outlookban](https://aka.ms/controlpf).
