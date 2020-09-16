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
ms.openlocfilehash: 27cc744bc57f1c18649e05c5b0df3b315c9c0201
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727245"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="20977-102">Késések a SharePoint-és OneDrive-értesítések fogadásakor</span><span class="sxs-lookup"><span data-stu-id="20977-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="20977-103">Először ellenőrizze a levélszemét vagy a Levélszemét mappát az e-mailben.</span><span class="sxs-lookup"><span data-stu-id="20977-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="20977-104">Ha a **több fájlból vagy tárból érkező összes értesítés késik**, keresse fel a [szolgáltatás állapota irányítópultot](https://portal.office.com/adminportal/home?ref=/servicehealth) , és ellenőrizze, hogy vannak-e olyan tanácsadók/incidensek, amelyek a SharePoint vagy az Exchange alkalmazásban esetleg előfordulnak.</span><span class="sxs-lookup"><span data-stu-id="20977-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="20977-105">Előfordulhat, hogy a probléma a SharePoint riasztási képességével vagy az e-mailek Exchange-ben való késésével jár.</span><span class="sxs-lookup"><span data-stu-id="20977-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="20977-106">Azt is megtudhatja, hogy az egyéb e-maileket kézbesíti-e, és ha nem, a probléma valószínűleg az Exchange késésekkel jár.</span><span class="sxs-lookup"><span data-stu-id="20977-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="20977-107">Ha **nincs kézbesítve egy adott fájl vagy tár egyéni figyelmeztetése**, próbálkozzon a törlésével és újbóli létrehozásával.</span><span class="sxs-lookup"><span data-stu-id="20977-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="20977-108">A riasztás újbóli létrehozásához olvassa el a [SharePoint-értesítések kezelése, megtekintése és törlése](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) című témakört.</span><span class="sxs-lookup"><span data-stu-id="20977-108">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="20977-109">Nem lehet értesítést küldeni a terjesztési csoportnak.</span><span class="sxs-lookup"><span data-stu-id="20977-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="20977-110">Csak a biztonsági és O365-csoportok támogatottak.</span><span class="sxs-lookup"><span data-stu-id="20977-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="20977-111">A riasztási e-mail-sablonok nem szabhatók testre.</span><span class="sxs-lookup"><span data-stu-id="20977-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="20977-112">Ezek eléréséhez a Microsoft flow vagy a SharePoint Designer munkafolyamatot kell használnia.</span><span class="sxs-lookup"><span data-stu-id="20977-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
