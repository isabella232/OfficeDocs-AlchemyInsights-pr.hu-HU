---
title: Nem kézbesítve a SharePoint riasztási értesítései
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: f4002dc865fb7a03b07a9256709b947d6d774cb0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751245"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a><span data-ttu-id="2b114-102">Nem kézbesítve a SharePoint riasztási értesítései</span><span class="sxs-lookup"><span data-stu-id="2b114-102">SharePoint alert notifications not delivered</span></span>

<span data-ttu-id="2b114-103">Jelölje be az e-mailek levélszemét mappáját, mert időnként riasztások is előfordulhatnak.</span><span class="sxs-lookup"><span data-stu-id="2b114-103">Please check the JUNK folder in your email, as sometimes alerts might go there.</span></span>

<span data-ttu-id="2b114-104">Annak megállapítása, hogy az **összes értesítés nem kézbesítve** van-e, illetve hogy nem kézbesíti-e az adott fájl vagy tár **Egyéni figyelmeztetését** .</span><span class="sxs-lookup"><span data-stu-id="2b114-104">Determine if **all alerts are not delivered** or if **an individual alert** from a specific file or library is not delivered.</span></span>

- <span data-ttu-id="2b114-105">A **rendszer nem kézbesíti az egyes riasztásokat**: Ha egy adott fájlból vagy tárból érkező egyéni figyelmeztetést nem kézbesítenek, akkor megkísérelheti törölni és újból létrehozni azt.</span><span class="sxs-lookup"><span data-stu-id="2b114-105">**Individual alerts are not delivered**: If an individual alert from a specific file or library is not delivered, you can attempt to delete and recreate it.</span></span> <span data-ttu-id="2b114-106">A riasztás újbóli létrehozásához olvassa el a [SharePoint-értesítések kezelése, megtekintése és törlése](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) című témakört.</span><span class="sxs-lookup"><span data-stu-id="2b114-106">See [Manage, view, or delete SharePoint alerts](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>
- <span data-ttu-id="2b114-107">A rendszer **nem kézbesíti az összes értesítést**: Ha a több fájlból vagy tárból származó összes értesítés nem érhető el, keresse fel a [szolgáltatás állapota irányítópultot](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , és ellenőrizze, hogy vannak-e olyan tanácsadók/incidensek, amelyek a SharePoint vagy az Exchange alkalmazásban esetleg előfordulnak.</span><span class="sxs-lookup"><span data-stu-id="2b114-107">**All alerts are not delivered**: If all alerts from multiple files or libraries are not delivered, visit the [Service Health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="2b114-108">A probléma lehet a SharePoint riasztási képessége vagy az e-mailek késése az Exchange-ben.</span><span class="sxs-lookup"><span data-stu-id="2b114-108">The issue could be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="2b114-109">Fontos tudni, hogy más e-maileket kézbesítenek-e, és ha nem, a probléma valószínűleg az Exchange késésekkel fog rendelkezni.</span><span class="sxs-lookup"><span data-stu-id="2b114-109">It will also be important to note whether other email is being delivered, and if not, the issue is likely with Exchange delays.</span></span>

<span data-ttu-id="2b114-110">Gyakori kérdések az értesítésekről:</span><span class="sxs-lookup"><span data-stu-id="2b114-110">FAQ on alerts:</span></span>

- <span data-ttu-id="2b114-111">Nem lehet értesítéseket küldeni a terjesztési csoportnak, csak a biztonsági és O365-csoportok támogatottak.</span><span class="sxs-lookup"><span data-stu-id="2b114-111">It is not possible to send alerts to Distribution Group, only Security and O365 groups are supported.</span></span>
- <span data-ttu-id="2b114-112">A riasztási e-mail-sablonok nem szabhatók testre; Ezek eléréséhez Microsoft FLOW vagy SharePoint Designer-munkafolyamatot kell használnia.</span><span class="sxs-lookup"><span data-stu-id="2b114-112">You cannot customize alert email templates; you need to use Microsoft FLOW or SharePoint Designer Workflow to achieve those.</span></span>

## <a name="related-topics"></a><span data-ttu-id="2b114-113">Kapcsolódó témakörök</span><span class="sxs-lookup"><span data-stu-id="2b114-113">Related Topics</span></span>

<span data-ttu-id="2b114-114">Szeretné kipróbálni a Microsoft flow-t a SharePoint Online-ban?</span><span class="sxs-lookup"><span data-stu-id="2b114-114">Want to try Microsoft Flow in SharePoint Online?</span></span>

- [<span data-ttu-id="2b114-115">Folyamatábra létrehozása</span><span class="sxs-lookup"><span data-stu-id="2b114-115">Create Flow</span></span>](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [<span data-ttu-id="2b114-116">SharePoint és flow</span><span class="sxs-lookup"><span data-stu-id="2b114-116">SharePoint and Flow</span></span>](https://flow.microsoft.com//blog/sharepoint-and-flow/)
