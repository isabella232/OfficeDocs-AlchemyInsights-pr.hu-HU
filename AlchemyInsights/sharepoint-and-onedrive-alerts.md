---
title: Késések a SharePoint-és OneDrive-értesítések fogadásakor
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 92e517ae6e83aa91b9838047ec77759dc893bc57
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/17/2020
ms.locfileid: "46785667"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="3ed63-102">Késések a SharePoint-és OneDrive-értesítések fogadásakor</span><span class="sxs-lookup"><span data-stu-id="3ed63-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="3ed63-103">Először ellenőrizze a levélszemét vagy a Levélszemét mappát az e-mailben.</span><span class="sxs-lookup"><span data-stu-id="3ed63-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="3ed63-104">Ha a **több fájlból vagy tárból érkező összes értesítés késik**, keresse fel a [szolgáltatás állapota irányítópultot](https://portal.office.com/adminportal/home?ref=/servicehealth) , és ellenőrizze, hogy vannak-e olyan tanácsadók/incidensek, amelyek a SharePoint vagy az Exchange alkalmazásban esetleg előfordulnak.</span><span class="sxs-lookup"><span data-stu-id="3ed63-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="3ed63-105">Előfordulhat, hogy a probléma a SharePoint riasztási képességével vagy az e-mailek Exchange-ben való késésével jár.</span><span class="sxs-lookup"><span data-stu-id="3ed63-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="3ed63-106">Azt is megtudhatja, hogy az egyéb e-maileket kézbesíti-e, és ha nem, a probléma valószínűleg az Exchange késésekkel jár.</span><span class="sxs-lookup"><span data-stu-id="3ed63-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="3ed63-107">Ha **nincs kézbesítve egy adott fájl vagy tár egyéni figyelmeztetése**, próbálkozzon a törlésével és újbóli létrehozásával.</span><span class="sxs-lookup"><span data-stu-id="3ed63-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="3ed63-108">A riasztás újbóli létrehozásához olvassa el a [SharePoint-értesítések kezelése, megtekintése és törlése](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) című témakört.</span><span class="sxs-lookup"><span data-stu-id="3ed63-108">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="3ed63-109">Nem lehet értesítést küldeni a terjesztési csoportnak.</span><span class="sxs-lookup"><span data-stu-id="3ed63-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="3ed63-110">Csak a biztonsági és O365-csoportok támogatottak.</span><span class="sxs-lookup"><span data-stu-id="3ed63-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="3ed63-111">A riasztási e-mail-sablonok nem szabhatók testre.</span><span class="sxs-lookup"><span data-stu-id="3ed63-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="3ed63-112">Ezek eléréséhez a Microsoft flow vagy a SharePoint Designer munkafolyamatot kell használnia.</span><span class="sxs-lookup"><span data-stu-id="3ed63-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
