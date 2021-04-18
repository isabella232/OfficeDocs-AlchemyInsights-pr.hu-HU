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
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816742"
---
# <a name="control-access-to-public-folders-using-outlook"></a>A nyilvános mappákhoz való hozzáférés szabályozása az Outlook használatával

A nyilvános mappákhoz hozzáférő felhasználók szabályozásához az Outlook használatával:

1. A `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false` használata

$true: Nyilvános mappák elérésének engedélyezése a felhasználóknak az Outlookban  
$false: A nyilvános mappák elérésének megakadályozása az Outlookban. Ez az alapértelmezett érték.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Megjegyzés: Ez az eljárás csak a Windows rendszerű asztali Outlook kapcsolatokat szabályozhatja. A felhasználók továbbra is hozzáférhetnek a nyilvános mappákhoz az OWA vagy a Mac Outlook használatával.

További információért lásd: [Ellenőrzött kapcsolatok a nyilvános mappákkal az Outlookban](https://aka.ms/controlpf).
