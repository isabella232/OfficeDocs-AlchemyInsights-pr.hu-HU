---
title: Bővítmények telepítése a Microsoft 365-alkalmazások
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233536"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>Bővítmények telepítése a Microsoft 365-alkalmazások

A Központi üzembe helyezés az ajánlott módszer a bővítmények Office és csoportok számára való telepítésére a szervezeten belül. Bővítmények telepítéséhez kövesse az alábbi lépéseket:

**Megjegyzés:** Ha egyéni felhasználóként szeretne Office bővítményt telepíteni, tekintse meg a Bővítmények megtekintése, kezelése és telepítése a Office [programokban Office.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d) Ezenkívül arról is győződjön meg, hogy a Office Áruházbeli bővítmények egyéni beszerzése engedélyezve van. Részletes információkért [lásd: Bővítmények](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)letöltésének megakadályozása az összes ügyfél Office (kivéve a Outlook).

1. Győződjön meg arról, hogy környezete megfelel a Bővítmények Központi üzembe helyezés használatával való telepítésének követelményeinek. Részletes információkért lásd: [Követelmények.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements)
2. A bővítmények **Gépház** telepítéséhez Gépház alkalmazások letöltése a Microsoft 365 Felügyeleti központban című  >    >   témakört. 

Megjegyzések: 

- Az integrált alkalmazások használatához a rendszergazdának globális rendszergazdai vagy rendszergazdai Exchange kell rendelkeznie.

- Amikor több felhasználónál telepíti a bővítményeket, azt javasoljuk, hogy az egyéni felhasználók helyett csoportok használatával vegyen fel hozzárendeléseket. Részletes információkért lásd: Megfontolandó szempontok a bővítmények felhasználókhoz [és csoportokhoz való hozzárendelése során.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)

- A Központi üzembe helyezés nem támogatja a beágyazott csoportok vagy szülőcsoportokkal csoportok felhasználóit. Részletes információkért lásd: [Felhasználó- és csoport-hozzárendelések.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)

- Győződjön meg arról, hogy a Microsoft 365 appkezelési szolgáltatás (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') engedélyezve van a felhasználók számára a bejelentkezéshez. Részletes információkért lásd: [Alkalmazástulajdonságok konfigurálása.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)

- Ha problémákat tapasztal a bővítmények integrált alkalmazások használatával való telepítése során, próbálkozzon azzal, hogy bővítményeket használ a [telepítéshez.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)

További információ:

[Bővítmények telepítése a Felügyeleti központban](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Bővítmények kezelése a Felügyeleti központban](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 Bővítmények kezelése a Központi üzembe helyezés [PowerShell-parancsmagokkal](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 Bővítmények Office Központi üzembe helyezés használatával a [Microsoft 365 felügyeleti központon keresztül](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Hibaelhárítás: A felhasználó nem látja a bővítményeket](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Felhasználói hibák elhárítása Office bővítményekkel](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)