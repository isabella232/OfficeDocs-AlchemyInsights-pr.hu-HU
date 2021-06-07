---
title: Webinárium-regisztráció kezelése
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
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793918"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="f0e7d-102">Webinárium-regisztráció kezelése</span><span class="sxs-lookup"><span data-stu-id="f0e7d-102">Manage webinar registration</span></span>

<span data-ttu-id="f0e7d-103">PowerShell-parancsokkal Teams kezelheti, hogy ki regisztrálhat Teams webináriumra.</span><span class="sxs-lookup"><span data-stu-id="f0e7d-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="f0e7d-104">A Powershell Teams való telepítéséhez lásd: [Teams PowerShell](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="f0e7d-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="f0e7d-105">A *WhoCanRegister* alapértelmezés szerint engedélyezve van, és a **EveryoneInCompany értéket adja meg.**</span><span class="sxs-lookup"><span data-stu-id="f0e7d-105">By default, *WhoCanRegister* is enabled and set to **EveryoneInCompany**.</span></span> <span data-ttu-id="f0e7d-106">Ahhoz, hogy bárki, beleértve a névtelen felhasználókat is,  regisztrálhat, az értekezleti házirendet Mindenki beállításra kell állítania a Powershell parancs használatával:</span><span class="sxs-lookup"><span data-stu-id="f0e7d-106">To allow anyone, including anonymous users, to register, you must set the Meeting Policy to **Everyone** by using the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="f0e7d-107">**Megjegyzés:** Ha a névtelen csatlakozás ki van kapcsolva az értekezlet beállításai között, a névtelen felhasználók nem csatlakozhatnak webináriumhoz.</span><span class="sxs-lookup"><span data-stu-id="f0e7d-107">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="f0e7d-108">További információért és a beállítás engedélyezéséről további információt az Értekezlet [beállításainak kezelése](/microsoftteams/meeting-settings-in-teams)a Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="f0e7d-108">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="f0e7d-109">Ha ki szeretné kapcsolni az értekezlet-regisztrációt, állítsa az *AllowMeetingRegistration értéket* **False (Hamis) beállításra.**</span><span class="sxs-lookup"><span data-stu-id="f0e7d-109">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="f0e7d-110">Ha többet szeretne megtudni arról, hogy ki regisztrálhat webináriumra, olvassa el A webináriumok regisztrálóira regisztrálók [konfigurálásacímet.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)</span><span class="sxs-lookup"><span data-stu-id="f0e7d-110">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="f0e7d-111">A Microsoft-listák beállításairól további információt A [Microsoft-listák beállításainak szabályozása](/sharepoint/control-lists)lapon található.</span><span class="sxs-lookup"><span data-stu-id="f0e7d-111">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
