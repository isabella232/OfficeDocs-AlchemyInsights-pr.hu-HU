---
title: Napló szerepkör hozzárendelése az Office 365 Biztonsági & megfelelőségi központban
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746169"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a><span data-ttu-id="49847-102">Napló szerepkör hozzárendelése az Office 365 Biztonsági & megfelelőségi központban</span><span class="sxs-lookup"><span data-stu-id="49847-102">Assign an Audit Log role in the Office 365 Security & Compliance Center</span></span>

<span data-ttu-id="49847-103">Az Office 365-naplóban való kereséshez egy rendszergazdának "Csak  megtekintési naplók" vagy "Naplók" szerepkört kell rendelnie az Exchange **Online-ban.**</span><span class="sxs-lookup"><span data-stu-id="49847-103">To search the Office 365 audit log, an administrator must be assigned the **View-Only Audit Logs** role or the **Audit Logs** role in Exchange Online.</span></span> <span data-ttu-id="49847-104">Ezek a szerepkörök alapértelmezés szerint a Megfelelőségkezelés és a Szervezetkezelés szerepkörcsoportokhoz vannak rendelve.</span><span class="sxs-lookup"><span data-stu-id="49847-104">These roles are assigned to the Compliance Management and Organization Management role groups by default.</span></span> <span data-ttu-id="49847-105">Az Office 365 és a Microsoft 365 globális rendszergazdái automatikusan felkerülnek a Szervezetkezelés szerepkörcsoport tagjaiként.</span><span class="sxs-lookup"><span data-stu-id="49847-105">Global administrators in Office 365 and Microsoft 365 are automatically added as members of the Organization Management role group.</span></span>

<span data-ttu-id="49847-106">Ha engedélyezni szeretné egy felhasználónak a minimális jogosultsági szinttel való keresést, hozzon létre egy  egyéni szerepkörcsoportot az Exchange **Online-ban,** vegye fel a Csak megtekintési naplók vagy a Naplók szerepkört, majd vegye fel a felhasználót az új szerepkörcsoport tagjaként.</span><span class="sxs-lookup"><span data-stu-id="49847-106">To enable a user to search with the minimum level of privileges, create a custom role group in Exchange Online, add the **View-Only Audit Logs** role or **Audit Logs** role, and then add the user as a member of the new role group.</span></span>

<span data-ttu-id="49847-107">További információt a Szerepkörcsoportok kezelése az [Exchange Online-ban](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) és a Naplókeresés a Biztonsági és [megfelelőségi központban &.](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)</span><span class="sxs-lookup"><span data-stu-id="49847-107">For more information, see [Manage role groups in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) and [Search the audit log in the Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>