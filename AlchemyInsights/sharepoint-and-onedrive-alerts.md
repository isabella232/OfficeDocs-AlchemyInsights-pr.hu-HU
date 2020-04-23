---
title: A SharePoint- és OneDrive-értesítések fogadásának késedelme
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: fb7ab6e8139c46d89b1cae1ee0ab9b9a601c8b64
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742003"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="5c440-102">A SharePoint- és OneDrive-értesítések fogadásának késedelme</span><span class="sxs-lookup"><span data-stu-id="5c440-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="5c440-103">Először ellenőrizze a Levélszemét vagy Spam mappát az e-mailben.</span><span class="sxs-lookup"><span data-stu-id="5c440-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="5c440-104">Ha **több fájl vagy tárak összes riasztása késik,** látogasson el a [Szolgáltatásállapot irányítópultjára,](https://portal.office.com/adminportal/home?ref=/servicehealth) és ellenőrizze, hogy vannak-e olyan tanácsok/incidensek, amelyek a SharePoint vagy az Exchange alkalmazásban előfordulhatnak.</span><span class="sxs-lookup"><span data-stu-id="5c440-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="5c440-105">A probléma lehet a SharePoint riasztási képesség vagy késedelmek e-mailek az Exchange-en keresztül.</span><span class="sxs-lookup"><span data-stu-id="5c440-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="5c440-106">Azt is vegye figyelembe, hogy más e-maileket kézbesítenek-e – ha nem, akkor a probléma valószínűleg az Exchange késéseivel van.</span><span class="sxs-lookup"><span data-stu-id="5c440-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="5c440-107">Ha **egy adott fájlból vagy tárból származó egyéni riasztás nem jelenik meg,** próbálja meg törölni és újra létrehozni.</span><span class="sxs-lookup"><span data-stu-id="5c440-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="5c440-108">A riasztás újbóli létrehozásához olvassa el A [SharePoint-értesítések kezelése, megtekintése és törlése](https://support.microsoft.com/office/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) című témakört.</span><span class="sxs-lookup"><span data-stu-id="5c440-108">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="5c440-109">Terjesztési csoportnak nem lehet értesítéseket küldeni.</span><span class="sxs-lookup"><span data-stu-id="5c440-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="5c440-110">Csak a Biztonság és az O365 csoportok támogatottak.</span><span class="sxs-lookup"><span data-stu-id="5c440-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="5c440-111">A figyelmeztető e-mail sablonok nem szabhatók testre.</span><span class="sxs-lookup"><span data-stu-id="5c440-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="5c440-112">Ezek eléréséhez microsoft flow vagy SharePoint Designer munkafolyamatot kell használnia.</span><span class="sxs-lookup"><span data-stu-id="5c440-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
