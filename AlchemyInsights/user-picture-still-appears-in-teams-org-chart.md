---
title: A felhasználói kép továbbra is megjelenik a Microsoft Teams diagramon
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13834"
- "9007457"
ms.openlocfilehash: be4c6feb55e6b7c4667566946d8d3640cc0ffb1d
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2021
ms.locfileid: "59422252"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>A felhasználói kép továbbra is megjelenik a Microsoft Teams diagramon

Ha a szervezetben egy vagy több személyt letiltottak vagy eltávolítottak, és a profilképük továbbra is megjelenik a szervezeti diagramon, lehetséges, hogy a **ShowInAddressLists** beállítás False (Hamis) van megállítva: 

1. Válassza Microsoft 365 Felügyeleti központ > Aktív [felhasználók lehetőséget,](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) és jelölje ki a még látható fényképet használó felhasználót. 
1. Válassza a **Levelek fület,** és győződjön meg arról, hogy **a Show in global address list (A** globális címlistában való megjelenítése) beállítás nemre **van állítva.**

Ha a **ShowInAddressLists** nem működik, ellenőrizze az alábbiakat:  

- Előfordulhat, hogy a felhasználó megjelenik a címzettek listájából a Exchange. További információt a Címlisták kezelése a [Exchange Online.](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists) 
- Előfordulhat, hogy a felhasználó megjelenik a Azure Active Directory. További információ: [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 