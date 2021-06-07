---
title: A Teams engedélyezése
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52793788"
---
# <a name="enable-teams-webinars"></a><span data-ttu-id="e9674-102">A Teams engedélyezése</span><span class="sxs-lookup"><span data-stu-id="e9674-102">Enable Teams Webinars</span></span>

<span data-ttu-id="e9674-103">A webináriumok alapértelmezés szerint engedélyezve vannak.</span><span class="sxs-lookup"><span data-stu-id="e9674-103">Webinars are enabled by default.</span></span> <span data-ttu-id="e9674-104">A PowerShell-parancsokkal Teams kezelheti, hogy ki ütemezhet és regisztrálhat Teams webináriumra.</span><span class="sxs-lookup"><span data-stu-id="e9674-104">You can manage who can schedule and register for Teams Webinars by using Teams PowerShell commands.</span></span>

- <span data-ttu-id="e9674-105">Az értekezletek létrehozására képes összes felhasználó is létrehozhat webinárium-értekezletet.</span><span class="sxs-lookup"><span data-stu-id="e9674-105">All users who can create a meeting can also create a webinar meeting.</span></span> <span data-ttu-id="e9674-106">Ha szeretné kezelni, hogy ki ütemezheti a Teams, használja az *AllowMeetingRegistration lehetőséget.*</span><span class="sxs-lookup"><span data-stu-id="e9674-106">If you want to manage who can schedule Teams Webinars, use *AllowMeetingRegistration*.</span></span> 
- <span data-ttu-id="e9674-107">A *WhoCanRegister* alapértelmezés szerint engedélyezve van, és Mindenki értéket **ad meg.**</span><span class="sxs-lookup"><span data-stu-id="e9674-107">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="e9674-108">Ha ki szeretné kapcsolni az értekezlet-regisztrációt, állítsa az *AllowMeetingRegistration értéket* **False (Hamis) beállításra.**</span><span class="sxs-lookup"><span data-stu-id="e9674-108">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="e9674-109">A beállítások módosításához telepítenie kell Teams [PowerShellt.](/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="e9674-109">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="e9674-110">Ezenkívül az értekezleti házirendek a webináriumok Teams is be vannak kényszerítve.</span><span class="sxs-lookup"><span data-stu-id="e9674-110">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="e9674-111">Ha például az értekezlet beállításaiban kikapcsolja a névtelen csatlakozást, a névtelen felhasználók nem csatlakozhatnak webináriumhoz.</span><span class="sxs-lookup"><span data-stu-id="e9674-111">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="e9674-112">Ha többet szeretne megtudni arról, hogy ki regisztrálhat webináriumra, olvassa el A webináriumok regisztrálóira regisztrálók [konfigurálásacímet.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)</span><span class="sxs-lookup"><span data-stu-id="e9674-112">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="e9674-113">A Microsoft-listák beállításairól további információt A [Microsoft-listák beállításainak szabályozása](/sharepoint/control-lists)lapon található.</span><span class="sxs-lookup"><span data-stu-id="e9674-113">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>