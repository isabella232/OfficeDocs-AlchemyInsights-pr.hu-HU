---
title: Klasszikus SharePoint-naplójelentések
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 0aedb549f11db54d3cd480671fb0767c60680ad3
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509602"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="32f63-102">A SharePoint és a OneDrive naplózási naplói</span><span class="sxs-lookup"><span data-stu-id="32f63-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="32f63-103">Klasszikus SharePoint-naplónaplók</span><span class="sxs-lookup"><span data-stu-id="32f63-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="32f63-104">Az SPO örökölt naplózása átlett telepítve az egyesített naplónaplóba (UAL).</span><span class="sxs-lookup"><span data-stu-id="32f63-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="32f63-105">Az összes SPO örökölt naplózási jelentés most antól az UAL-n keresztül lesz, és az örökölt naplózási jelek átlettek telepítve az UAL-ba.</span><span class="sxs-lookup"><span data-stu-id="32f63-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="32f63-106">Legfontosabb változások:</span><span class="sxs-lookup"><span data-stu-id="32f63-106">Key changes:</span></span>

* <span data-ttu-id="32f63-107">A vágás nem érhető el képességként.</span><span class="sxs-lookup"><span data-stu-id="32f63-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="32f63-108">A naplózandó események kiválasztása NEM érhető el.</span><span class="sxs-lookup"><span data-stu-id="32f63-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="32f63-109">Ebben a [dokumentumban](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) az alapértelmezés szerint elérhető naplózott események teljes listáját tartalmazza.</span><span class="sxs-lookup"><span data-stu-id="32f63-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="32f63-110">A **Hely** beállítás a **Testreszabott jelentések** csoportban NEM érhető el.</span><span class="sxs-lookup"><span data-stu-id="32f63-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="32f63-111">A **dokumentumok megnyitása vagy letöltése** események nem érhető el.</span><span class="sxs-lookup"><span data-stu-id="32f63-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="32f63-112">Webhelycsoport naplózási beállításainak konfigurálása</span><span class="sxs-lookup"><span data-stu-id="32f63-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="32f63-113">A SharePoint és a OneDrive modern, egységes naplózási naplói a megfelelőségből</span><span class="sxs-lookup"><span data-stu-id="32f63-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="32f63-114">Az egyesített naplózás be- és kikapcsolása</span><span class="sxs-lookup"><span data-stu-id="32f63-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="32f63-115">Nincs szükség további konfigurációra a SharePointban vagy a OneDrive-on belül.</span><span class="sxs-lookup"><span data-stu-id="32f63-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="32f63-116">A naplózási keresés sel ellenőrizheti a fájl(ok), a mappa(ok), a felhasználó(k), az engedélyek tevékenységét:</span><span class="sxs-lookup"><span data-stu-id="32f63-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="32f63-117">Fájl- és oldaltevékenységek</span><span class="sxs-lookup"><span data-stu-id="32f63-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="32f63-118">Mappatevékenységek</span><span class="sxs-lookup"><span data-stu-id="32f63-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="32f63-119">Megosztási és hozzáférési kérelmekkel kapcsolatos tevékenységek</span><span class="sxs-lookup"><span data-stu-id="32f63-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="32f63-120">Szinkronizálási tevékenységek</span><span class="sxs-lookup"><span data-stu-id="32f63-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="32f63-121">Webhely-adminisztrációs tevékenységek</span><span class="sxs-lookup"><span data-stu-id="32f63-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="32f63-122">Az események beolvasásáról a [Keresés a naplóban](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)című témakörben talál további információt.</span><span class="sxs-lookup"><span data-stu-id="32f63-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
