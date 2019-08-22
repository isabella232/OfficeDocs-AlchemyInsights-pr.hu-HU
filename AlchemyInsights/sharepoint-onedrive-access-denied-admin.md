---
title: A hozzáférés megtagadva üzenetet – problémamegoldás
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 0a885e15d54c9337711f2528628789dfcb903264
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36503531"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="89c7c-102">Üzenetek megtagadta a hozzáférést a Sharepoint/OneDrive Admin Center – problémamegoldás</span><span class="sxs-lookup"><span data-stu-id="89c7c-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="89c7c-103">Ha a hozzáférés megtagadásáról, tallózással keresse meg a Sharepoint/OneDrive Admin Center megkísérelte kap, győződjön meg arról, hogy [a felhasználó licenc hozzárendelése](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="89c7c-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="89c7c-104">Ha a felhasználói licenccel rendelkezik, akkor győződjön meg arról is [egy rendszergazda szerepkört](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) , amelyhez hozzáférhet az admin-centers.</span><span class="sxs-lookup"><span data-stu-id="89c7c-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="89c7c-105">Ez a probléma akkor is előfordulhat, amikor a felhasználó törli, és újra létrehozza a ugyanolyan egyszerű felhasználónév (UPN).</span><span class="sxs-lookup"><span data-stu-id="89c7c-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="89c7c-106">Az új fiók jön létre egy másik értéket PUID (Passport egyedi azonosító) segítségével.</span><span class="sxs-lookup"><span data-stu-id="89c7c-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="89c7c-107">Ha a felhasználó megpróbál hozzáférni egy webhelycsoport vagy a OneDrive, a felhasználó rendelkezik egy helytelen PUID.</span><span class="sxs-lookup"><span data-stu-id="89c7c-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="89c7c-108">A második forgatókönyv magában foglalja a könyvtár szinkronizálás az Active Directory szervezeti egységet (OU).</span><span class="sxs-lookup"><span data-stu-id="89c7c-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="89c7c-109">Ha a felhasználó rendelkezik már bejelentkezett a SharePoint, majd átkerül egy másik szervezeti egység és SharePoint resynced, akkor ez a probléma tapasztalhatnak.</span><span class="sxs-lookup"><span data-stu-id="89c7c-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="89c7c-110">A probléma megoldásához a cikk [az Office 365 rendszerben a felhasználó visszaállítási](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)lépéseket az eredeti UPN kell visszaállítani.</span><span class="sxs-lookup"><span data-stu-id="89c7c-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="89c7c-111">Megjegyzés: Ha több felhasználónak, aki korábban a hozzáférést a OneDrive vagy a SharePoint felügyeleti központ nem érhető el, lehet egy ideiglenes szolgáltatást a probléma.</span><span class="sxs-lookup"><span data-stu-id="89c7c-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="89c7c-112">[Ellenőrizze a szolgáltatás egészségügyi irányítópult](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="89c7c-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


