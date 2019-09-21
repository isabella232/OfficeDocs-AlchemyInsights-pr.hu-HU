---
title: Klasszikus SharePoint-Naplójelentések
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068025"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="10745-102">SharePoint és OneDrive naplónapló</span><span class="sxs-lookup"><span data-stu-id="10745-102">SharePoint and OneDrive audit logs</span></span>

<span data-ttu-id="10745-103">**SharePoint és OneDrive modern egyesített audit naplók a megfelelőségi**</span><span class="sxs-lookup"><span data-stu-id="10745-103">**SharePoint and OneDrive Modern Unified Audit logs from compliance**</span></span>

- [<span data-ttu-id="10745-104">Az egyesített Naplónaplózás be-és kikapcsolása</span><span class="sxs-lookup"><span data-stu-id="10745-104">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="10745-105">Nincs szükség további konfigurálást a SharePoint vagy az OneDrive belül.</span><span class="sxs-lookup"><span data-stu-id="10745-105">No additional configuration is required within SharePoint or OneDrive.</span></span>

- <span data-ttu-id="10745-106">A naplóvizsgálat kereséssel ellenőrizheti a fájl (ok), a mappa (ok), a felhasználó (k) és az engedélyek használatát.</span><span class="sxs-lookup"><span data-stu-id="10745-106">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

    - [<span data-ttu-id="10745-107">Fájl-és oldaltevékenységek</span><span class="sxs-lookup"><span data-stu-id="10745-107">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [<span data-ttu-id="10745-108">Mappatevékenységek</span><span class="sxs-lookup"><span data-stu-id="10745-108">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [<span data-ttu-id="10745-109">Kérésmegosztási és hozzáférési tevékenységek</span><span class="sxs-lookup"><span data-stu-id="10745-109">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [<span data-ttu-id="10745-110">Szinkronizálási tevékenységek</span><span class="sxs-lookup"><span data-stu-id="10745-110">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [<span data-ttu-id="10745-111">Webhely-adminisztrációs tevékenységek</span><span class="sxs-lookup"><span data-stu-id="10745-111">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- <span data-ttu-id="10745-112">További információt az események lekéréséről [a naplózás keresése](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="10745-112">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="10745-113">**Klasszikus SharePoint-naplófájlok**</span><span class="sxs-lookup"><span data-stu-id="10745-113">**SharePoint classic Audit logs**</span></span>

<span data-ttu-id="10745-114">Áttelepítette az SPO örökölt naplózását az egyesített Naplónaplóra (UAL).</span><span class="sxs-lookup"><span data-stu-id="10745-114">We migrated SPO legacy auditing to Unified Audit Log (UAL).</span></span> <span data-ttu-id="10745-115">Ez lényegében azt jelenti, hogy minden SPO örökölt ellenőrzési jelentések most hajtott keresztül UAL, és a korábbi vizsgálati jelek átkerültek UAL.</span><span class="sxs-lookup"><span data-stu-id="10745-115">This essentially means that all SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="10745-116">Kulcs megváltozik:</span><span class="sxs-lookup"><span data-stu-id="10745-116">Key changes:</span></span>

- <span data-ttu-id="10745-117">A kivágás mint képesség nem áll rendelkezésre.</span><span class="sxs-lookup"><span data-stu-id="10745-117">Trimming as a capability is NOT available.</span></span>
- <span data-ttu-id="10745-118">NEM érhető el az a szakasz, amelyben a naplózni kívánt eseményeket kiválasztja.</span><span class="sxs-lookup"><span data-stu-id="10745-118">The section where you choose specific events to audit is NOT available.</span></span> <span data-ttu-id="10745-119">Kérjük, olvassa el [ezt a dokumentumot](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) az alapértelmezetten elérhető naplózott események teljes listájért.</span><span class="sxs-lookup"><span data-stu-id="10745-119">Please refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
- <span data-ttu-id="10745-120">A **testreszabott jelentések** alatt lévő "hely" beállítás nem érhető el.</span><span class="sxs-lookup"><span data-stu-id="10745-120">The "Location" option under **Customized reports** is NOT available.</span></span> 
- <span data-ttu-id="10745-121">"Dokumentumok megnyitása vagy letöltése" események nem érhetők el.</span><span class="sxs-lookup"><span data-stu-id="10745-121">“Opening or downloading documents” events is NOT available.</span></span> 

