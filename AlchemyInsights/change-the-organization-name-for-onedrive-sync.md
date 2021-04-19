---
title: A OneDrive szinkronizálási ügyfélalkalmazás szervezetnevének módosítása
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
- "9003077"
- "5850"
ms.openlocfilehash: ca545ba51e39209f3302acdee1c24048515e2c1b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818326"
---
# <a name="change-the-organization-name-for-the-onedrive-sync-client"></a><span data-ttu-id="743a8-102">A OneDrive szinkronizálási ügyfélalkalmazás szervezetnevének módosítása</span><span class="sxs-lookup"><span data-stu-id="743a8-102">Change the organization name for the OneDrive sync client</span></span>

<span data-ttu-id="743a8-103">A OneDrive a bérlői rendszergazda által beállított szervezetnevet használja.</span><span class="sxs-lookup"><span data-stu-id="743a8-103">OneDrive uses the organization name set by a tenant administrator.</span></span>  <span data-ttu-id="743a8-104">Módosíthatja a szervezet címét, műszaki [kapcsolattartóját és sok mását.](https://docs.microsoft.com/microsoft-365/admin/manage/change-address-contact-and-more)</span><span class="sxs-lookup"><span data-stu-id="743a8-104">You can [change your organization's address, technical contact, and more](https://docs.microsoft.com/microsoft-365/admin/manage/change-address-contact-and-more).</span></span> <span data-ttu-id="743a8-105">Miután végrehajtotta a változtatást a bérlői fiókban, a OneDrive szinkronizálási ügyfélalkalmazás mindaddig nem fogja tükrözni az új nevet, amíg a felhasználók le nem leválasztják, majd újra nem csatolják OneDrive-fiókjukat.</span><span class="sxs-lookup"><span data-stu-id="743a8-105">Once that change is performed for the tenant, the OneDrive sync client will not reflect the new name until users unlink and relink their OneDrive account.</span></span>

<span data-ttu-id="743a8-106">A fiók leválasztása:</span><span class="sxs-lookup"><span data-stu-id="743a8-106">To unlink the account:</span></span>

1. <span data-ttu-id="743a8-107">Válassza a onedrive kék felhőikonját a tálca jobb szélén, majd válassza a További beállítások > **Beállítások > lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="743a8-107">Select the blue OneDrive cloud icon at the far right of the taskbar, then select  **More > Settings > Account**.</span></span>
2. <span data-ttu-id="743a8-108">Keresse meg a leválasztni kívánt fiókot, és válassza a Számítógép leválasztása **,** majd a Fiók **leválasztása lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="743a8-108">Find the account you want to unlink and select  **Unlink this PC**, and then  **Unlink account**.</span></span>

<span data-ttu-id="743a8-109">A fiók újra kapcsolatba hozása:  válassza a Fiók hozzáadása lehetőséget **a** Beállítások lap Fiók lapján, és jelentkezzen be újra a OneDrive-ba.</span><span class="sxs-lookup"><span data-stu-id="743a8-109">To relink the account, select  **Add an account** from the  **Account** tab in Settings, and sign back into OneDrive.</span></span>