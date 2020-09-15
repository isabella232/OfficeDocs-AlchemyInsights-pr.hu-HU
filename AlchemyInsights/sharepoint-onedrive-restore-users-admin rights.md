---
title: A OneDrive vállalati verziós webhelyekhez való hozzáférés megtagadását jelző üzenetek hibaelhárítása
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670618"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="5053c-102">A OneDrive vállalati verziós webhelyekhez való hozzáférés megtagadását jelző üzenetek hibaelhárítása</span><span class="sxs-lookup"><span data-stu-id="5053c-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="5053c-103">Ez a probléma leggyakrabban akkor fordul elő, ha egy felhasználó törlődik, és a felhasználó ugyanazzal a egyszerű névvel (UPN) jön létre újra.</span><span class="sxs-lookup"><span data-stu-id="5053c-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="5053c-104">Az új fiókot egy másik PUID (Passport egyedi azonosító) használatával hozza létre.</span><span class="sxs-lookup"><span data-stu-id="5053c-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="5053c-105">Amikor a felhasználó megkísérel hozzáférni egy webhelycsoportban vagy a OneDrive, a felhasználó helytelen PUID rendelkezik.</span><span class="sxs-lookup"><span data-stu-id="5053c-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="5053c-106">A második forgatókönyv a címtár-szinkronizálást jelenti Active Directory-beli szervezeti egységgel (OU).</span><span class="sxs-lookup"><span data-stu-id="5053c-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="5053c-107">Ha a felhasználók már bejelentkezett a SharePointba, és egy másik szervezeti egységbe vannak áthelyezve, és a SharePointtal újra szinkronizálják őket, előfordulhat, hogy ez a probléma tapasztalható.</span><span class="sxs-lookup"><span data-stu-id="5053c-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="5053c-108">A probléma megoldásához vissza kell állítania az eredeti UPN-t a cikkben ismertetett lépésekkel, ha [vissza szeretne állítani egy felhasználót a Microsoft 365-ban](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="5053c-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
2. <span data-ttu-id="5053c-109">Ha nem tudja visszaállítani az eredeti felhasználót, a fenti lépésekkel távolítsa el a régi felhasználót a OneDrive webhelyről, [távolítsa el a felhasználót a felhasználói adatok listából]().</span><span class="sxs-lookup"><span data-stu-id="5053c-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="5053c-110">Miután ezt megtette, ellenőrizheti, hogy a felhasználó rendszergazdai jogosultságokkal rendelkezik-e a OneDrive-webhelyhez a [rendszergazda hozzáadása a felhasználó OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles) című témakör lépéseit követve.</span><span class="sxs-lookup"><span data-stu-id="5053c-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="5053c-111">A jogosultsági szintekről a [SharePoint jogosultsági szintjeinek ismertetése](https://docs.microsoft.com/sharepoint/understanding-permission-levels)című témakörben olvashat bővebben.</span><span class="sxs-lookup"><span data-stu-id="5053c-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
