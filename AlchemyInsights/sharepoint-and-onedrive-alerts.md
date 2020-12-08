---
title: Késések a SharePoint-és OneDrive-értesítések fogadásakor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: e5476f4e8462f233ff2a46832742d5a1f6e14e73
ms.sourcegitcommit: 38c87ed786dda7181562492d5d2e7ef0e18e0cab
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599854"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="ef4a8-102">Késések a SharePoint-és OneDrive-értesítések fogadásakor</span><span class="sxs-lookup"><span data-stu-id="ef4a8-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="ef4a8-103">Ha a **több fájlból vagy tárból érkező összes értesítés késik**, keresse fel a [szolgáltatás állapota irányítópultot](https://portal.office.com/adminportal/home?ref=/servicehealth) , és ellenőrizze, hogy vannak-e olyan tanácsadók/incidensek, amelyek a SharePoint vagy az Exchange alkalmazásban esetleg előfordulnak.</span><span class="sxs-lookup"><span data-stu-id="ef4a8-103">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span>
- <span data-ttu-id="ef4a8-104">Ha **nincs kézbesítve egy adott fájl vagy tár egyéni figyelmeztetése**, próbálkozzon a törlésével és újbóli létrehozásával.</span><span class="sxs-lookup"><span data-stu-id="ef4a8-104">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="ef4a8-105">A riasztás újbóli létrehozásához olvassa el a [SharePoint-értesítések kezelése, megtekintése és törlése](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) című témakört.</span><span class="sxs-lookup"><span data-stu-id="ef4a8-105">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>
- <span data-ttu-id="ef4a8-106">Ellenőrizze az e-mailben a levélszemét vagy a Levélszemét mappát.</span><span class="sxs-lookup"><span data-stu-id="ef4a8-106">Check the Junk or Spam folder in your email.</span></span>

> [!NOTE]
> - <span data-ttu-id="ef4a8-107">Nem lehet értesítést küldeni a terjesztési csoportnak.</span><span class="sxs-lookup"><span data-stu-id="ef4a8-107">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="ef4a8-108">Csak a biztonsági és O365-csoportok támogatottak.</span><span class="sxs-lookup"><span data-stu-id="ef4a8-108">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="ef4a8-109">A riasztási e-mail-sablonok nem szabhatók testre.</span><span class="sxs-lookup"><span data-stu-id="ef4a8-109">You cannot customize alert email templates.</span></span> <span data-ttu-id="ef4a8-110">Ezek eléréséhez a Microsoft flow vagy a SharePoint Designer munkafolyamatot kell használnia.</span><span class="sxs-lookup"><span data-stu-id="ef4a8-110">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
