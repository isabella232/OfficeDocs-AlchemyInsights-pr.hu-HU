---
title: 286--naplózásának engedélyezése
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "286"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 84794755f7756838393f11d617fcc8a5e3748e9f
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35388463"
---
# <a name="search-the-audit-log"></a><span data-ttu-id="ca6f4-102">Keresés a naplóban</span><span class="sxs-lookup"><span data-stu-id="ca6f4-102">Search the audit log</span></span>

<span data-ttu-id="ca6f4-103">Az Office 365 napló megkereséséhez kövesse az [alábbi lépéseket](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="ca6f4-103">To search the Office 365 audit log, follow [these steps](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="ca6f4-104">**Exchange**</span><span class="sxs-lookup"><span data-stu-id="ca6f4-104">**Exchange**</span></span>

- <span data-ttu-id="ca6f4-105">Az Exchange felügyeleti tevékenységek alapértelmezés szerint naplózza a rendszer.</span><span class="sxs-lookup"><span data-stu-id="ca6f4-105">Exchange admin activities are audited by default.</span></span>

- <span data-ttu-id="ca6f4-106">Mindannyian postaláda alapértelmezés szerint az Office 365 naplózásának engedélyezése során.</span><span class="sxs-lookup"><span data-stu-id="ca6f4-106">We are in the process of enabling mailbox auditing by default in Office 365.</span></span> <span data-ttu-id="ca6f4-107">Addig postafiók vagy a szervezet összes postaládáját naplózásának engedélyezéséhez [e cikkében](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)talál.</span><span class="sxs-lookup"><span data-stu-id="ca6f4-107">Until then, to enable auditing for a single mailbox or for all mailboxes in your organization, see  [this article](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing).</span></span>

- <span data-ttu-id="ca6f4-108">Office 365 csoport postafiókokat és nyilvános mappa postafiókok Exchange online nem támogatják a naplózás.</span><span class="sxs-lookup"><span data-stu-id="ca6f4-108">Office 365 Group mailboxes and public folder mailboxes in Exchange Online don't support audit logging.</span></span>

<span data-ttu-id="ca6f4-109">**SharePoint- és OneDrive**</span><span class="sxs-lookup"><span data-stu-id="ca6f4-109">**SharePoint and OneDrive**</span></span>

- <span data-ttu-id="ca6f4-110">Nincs SharePoint és OneDrive naplózásának engedélyezéséhez szükséges további konfigurálásra.</span><span class="sxs-lookup"><span data-stu-id="ca6f4-110">There's no additional configuration required to enable auditing for SharePoint and OneDrive.</span></span>

- <span data-ttu-id="ca6f4-111">SharePoint- és OneDrive támogatja a következő típusú tevékenységek naplózása:</span><span class="sxs-lookup"><span data-stu-id="ca6f4-111">SharePoint and OneDrive support auditing the following types of activities:</span></span>

    - <span data-ttu-id="ca6f4-112">Fájl, mappa és a tevékenységek lap</span><span class="sxs-lookup"><span data-stu-id="ca6f4-112">File, folder, and page activities</span></span>
    - <span data-ttu-id="ca6f4-113">Megosztása és a hozzáférési kérelem tevékenységek</span><span class="sxs-lookup"><span data-stu-id="ca6f4-113">Sharing and access request activities</span></span>
    - <span data-ttu-id="ca6f4-114">Webhely-felügyeleti tevékenységek</span><span class="sxs-lookup"><span data-stu-id="ca6f4-114">Site administration activities</span></span>
    - <span data-ttu-id="ca6f4-115">Fájl szinkronizálási tevékenységek</span><span class="sxs-lookup"><span data-stu-id="ca6f4-115">File synchronization activities</span></span>

- <span data-ttu-id="ca6f4-116">Más Office 365 szolgáltatások ellenőrzött tevékenységeivel kapcsolatos tudnivalókért tanulmányozza [a jelen cikkben szereplő táblázatot](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities).</span><span class="sxs-lookup"><span data-stu-id="ca6f4-116">For information about audited activities in other Office 365 services, see  [the table in this article](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities).</span></span>

- <span data-ttu-id="ca6f4-117">Gyakori kérdések [gyakran ismételt kérdések](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#frequently-asked-questions) a napló keresése itt.</span><span class="sxs-lookup"><span data-stu-id="ca6f4-117">Here a list of frequently asked questions [frequently asked questions](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#frequently-asked-questions) about searching the audit log.</span></span>