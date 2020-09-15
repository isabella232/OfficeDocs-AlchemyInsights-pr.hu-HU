---
title: Klasszikus SharePoint-naplózási jelentések
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662210"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="6d020-102">A SharePoint és a OneDrive naplói</span><span class="sxs-lookup"><span data-stu-id="6d020-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="6d020-103">Klasszikus SharePoint-napló</span><span class="sxs-lookup"><span data-stu-id="6d020-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="6d020-104">A Spongya örökölt naplózását az egyesített naplóba (UAL) migrálták.</span><span class="sxs-lookup"><span data-stu-id="6d020-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="6d020-105">Mostantól az összes, a UAL-on keresztül megjelenő régi naplózási jelentés átkerül a UAL-ba.</span><span class="sxs-lookup"><span data-stu-id="6d020-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="6d020-106">Főbb változások:</span><span class="sxs-lookup"><span data-stu-id="6d020-106">Key changes:</span></span>

* <span data-ttu-id="6d020-107">A körülvágás nem használható lehetőségként.</span><span class="sxs-lookup"><span data-stu-id="6d020-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="6d020-108">A naplózandó események kiválasztása nem érhető el.</span><span class="sxs-lookup"><span data-stu-id="6d020-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="6d020-109">Ebben a [dokumentumban](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) az alapértelmezés szerint elérhető naplózási események teljes listáját tekintheti meg.</span><span class="sxs-lookup"><span data-stu-id="6d020-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="6d020-110">A **testre szabott jelentések** területen a **hely** lehetőség nem érhető el.</span><span class="sxs-lookup"><span data-stu-id="6d020-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="6d020-111">A **dokumentumok megnyitása és letöltése** eseményekhez lehetőség nem érhető el.</span><span class="sxs-lookup"><span data-stu-id="6d020-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="6d020-112">Webhelycsoport naplózási beállításainak megadása</span><span class="sxs-lookup"><span data-stu-id="6d020-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="6d020-113">A SharePoint és a OneDrive modern, egységes könyvvizsgálati naplók a megfelelőségi szolgáltatásból</span><span class="sxs-lookup"><span data-stu-id="6d020-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="6d020-114">Az egyesített naplózás be-és kikapcsolása</span><span class="sxs-lookup"><span data-stu-id="6d020-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="6d020-115">A SharePointban és az OneDrive-ban nincs szükség további konfigurálásra.</span><span class="sxs-lookup"><span data-stu-id="6d020-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="6d020-116">A naplózás naplózása szolgáltatással ellenőrizheti a fájl (ok), a mappa (ok), a felhasználó (k) és az engedélyek működését:</span><span class="sxs-lookup"><span data-stu-id="6d020-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="6d020-117">Fájlok és lapok tevékenysége</span><span class="sxs-lookup"><span data-stu-id="6d020-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="6d020-118">Mappákkal kapcsolatos tevékenységek</span><span class="sxs-lookup"><span data-stu-id="6d020-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="6d020-119">Megosztási és hozzáférés-kérési tevékenységek</span><span class="sxs-lookup"><span data-stu-id="6d020-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="6d020-120">Szinkronizálási tevékenységek</span><span class="sxs-lookup"><span data-stu-id="6d020-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="6d020-121">Webhely-felügyeleti tevékenységek</span><span class="sxs-lookup"><span data-stu-id="6d020-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="6d020-122">Ha többet szeretne tudni az események beolvasásáról, olvassa el [a keresés a naplóban](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)című témakört.</span><span class="sxs-lookup"><span data-stu-id="6d020-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
