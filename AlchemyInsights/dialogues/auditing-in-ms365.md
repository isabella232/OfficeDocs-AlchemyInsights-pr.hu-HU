---
title: Naplózás a Microsoft 365-ben
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: c07981bfae40d74deb1a2f143ce51da69b51a69f
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429649"
---
# <a name="auditing-in-microsoft-365"></a><span data-ttu-id="d258d-102">Naplózás a Microsoft 365-ben</span><span class="sxs-lookup"><span data-stu-id="d258d-102">Auditing in Microsoft 365</span></span>

<span data-ttu-id="d258d-103">Íme néhány dolog, amit érdemes tudnia a Microsoft 365 naplózásával kapcsolatban:</span><span class="sxs-lookup"><span data-stu-id="d258d-103">Here are a few things you should know about auditing in Microsoft 365:</span></span>

1. <span data-ttu-id="d258d-104">Az Exchange-rendszergazdai tevékenységek naplózása alapértelmezés szerint meg van jelölve.</span><span class="sxs-lookup"><span data-stu-id="d258d-104">Exchange admin activities are audited by default.</span></span>
1. <span data-ttu-id="d258d-105">Folyamatban van a postaláda-naplózás alapértelmezés szerint bekapcsolása az összes felhasználónál.</span><span class="sxs-lookup"><span data-stu-id="d258d-105">We're in the process of turning on mailbox auditing by default for all users.</span></span> <span data-ttu-id="d258d-106">További információért kattintson [ide.](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Exchange-Mailbox-Auditing-will-be-enabled-by-default/ba-p/215171)</span><span class="sxs-lookup"><span data-stu-id="d258d-106">To read more about this, click [here](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Exchange-Mailbox-Auditing-will-be-enabled-by-default/ba-p/215171).</span></span> <span data-ttu-id="d258d-107">Addig is, ha azt szeretné, hogy az utasításokat manuálisan engedélyezze egy személy vagy egy teljes szervezet számára, válassza az alábbi Postaláda-naplózás bekapcsolása gombot.</span><span class="sxs-lookup"><span data-stu-id="d258d-107">Until then, if you want instructions to manually enable it for one person or an entire organization, choose the Turn on mailbox auditing button below.</span></span>
1. <span data-ttu-id="d258d-108">A Microsoft 365-csoportok postaládái és a nyilvánosmappa-postaládák nem támogatják a naplózást.</span><span class="sxs-lookup"><span data-stu-id="d258d-108">Microsoft 365 Groups mailboxes and Public Folder mailboxes do not support audit logging.</span></span>
1. <span data-ttu-id="d258d-109">A SharePoint/OneDrive esetén nincs szükség további konfigurációra a naplózás engedélyezett beállításához.</span><span class="sxs-lookup"><span data-stu-id="d258d-109">For SharePoint/OneDrive, there is no additional configuration required to enabled auditing.</span></span> <span data-ttu-id="d258d-110">A naplóban végzett tevékenységekről a következő cikkből olvashat:</span><span class="sxs-lookup"><span data-stu-id="d258d-110">To learn what activities are audited, see:</span></span>
    1. [<span data-ttu-id="d258d-111">Fájltevékenységek</span><span class="sxs-lookup"><span data-stu-id="d258d-111">File activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#file-and-page-activities)
    1. [<span data-ttu-id="d258d-112">Mappatevékenységek</span><span class="sxs-lookup"><span data-stu-id="d258d-112">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    1. <span data-ttu-id="d258d-113">[Megosztási és hozzáférési tevékenységek.](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)</span><span class="sxs-lookup"><span data-stu-id="d258d-113">[Sharing and Access activities](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities).</span></span>
1. <span data-ttu-id="d258d-114">A szolgáltatás szerint naplóolt tevékenységek listáját a Naplós [tevékenységek között láthatja.](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities)</span><span class="sxs-lookup"><span data-stu-id="d258d-114">For a list of all audited activities by service, see [Audited activities](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities).</span></span>
