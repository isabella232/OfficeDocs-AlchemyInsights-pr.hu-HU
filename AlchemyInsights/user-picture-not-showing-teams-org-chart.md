---
title: A felhasználói kép nem jelenik meg Microsoft Teams szervezeti diagramon
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/23/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12620"
- "9007457"
ms.openlocfilehash: 661b04913581ddd6650316298134ff9835ef3a90
ms.sourcegitcommit: 3986fa5377895cfc9fd98aca0739e599ebafb712
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/23/2021
ms.locfileid: "58792756"
---
# <a name="user-picture-not-showing-in-microsoft-teams-organization-chart"></a>A felhasználói kép nem jelenik meg Microsoft Teams szervezeti diagramon

Ha a szervezetben egy vagy több személynél hiányzik a profilképe a szervezeti diagramon, lehetséges, hogy a **ShowInAddressLists** beállítás False (Hamis) értékre **van állítva:**

1. Válassza Microsoft 365 Felügyeleti központ > Aktív [**felhasználók lehetőséget,**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)és jelölje ki a hiányzó fényképet használó felhasználót. 
1. Válassza a **Levelek fület,** és győződjön meg arról, hogy **a Show in global address list (A** globális címlistában való megjelenítése) beállítás igenre **van állítva.** 

Ha a **ShowInAddressLists** beállítás nem működik, ellenőrizze az alábbiakat: 

- Előfordulhat, hogy a felhasználó el van rejtve a címzettek listájáról Exchange. További információt a Címlisták kezelése a [Exchange Online.](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists) 
- Előfordulhat, hogy a felhasználó el van rejtve a Azure Active Directory. További információ: [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 
