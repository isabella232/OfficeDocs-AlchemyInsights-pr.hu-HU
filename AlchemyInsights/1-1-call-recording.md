---
title: 1:1-es hívásrögzítés
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733851"
---
# <a name="11-call-recording"></a><span data-ttu-id="37ca3-102">1:1-es hívásrögzítés</span><span class="sxs-lookup"><span data-stu-id="37ca3-102">1:1 call recording</span></span>

<span data-ttu-id="37ca3-103">A rendszergazdáknak azonnal el kell fogadnia a szükséges lépéseket ahhoz, hogy a felhasználók folytathatják az 1:1-es hívások rögzítését.</span><span class="sxs-lookup"><span data-stu-id="37ca3-103">Administrators need to take action now to continue allowing users to Record 1:1 calls.</span></span>
 
<span data-ttu-id="37ca3-104">2021. április 12-től kezdve bevezetjük az *AllowCloudRecordingForCalls* új Teams-hívási házirend-beállítását.</span><span class="sxs-lookup"><span data-stu-id="37ca3-104">Beginning April 12, 2021, we will start enforcing a new Teams Calling Policy option *AllowCloudRecordingForCalls*.</span></span> 

<span data-ttu-id="37ca3-105">A hívásrögzítési funkciókat jelenleg a Teams-értekezleti házirendek *AllowCloudRecording* beállításával lehet vezérelni.</span><span class="sxs-lookup"><span data-stu-id="37ca3-105">Currently 1:1 call recording capabilities are controlled by the *AllowCloudRecording* option in Teams Meeting Policies.</span></span> <span data-ttu-id="37ca3-106">Ha a felhasználóknak engedélyezett a Teams-értekezletek rögzítésére, az egy:1-es hívásokat is rögzíthetnek.</span><span class="sxs-lookup"><span data-stu-id="37ca3-106">If your users are allowed to record Teams Meetings they can also record 1:1 calls.</span></span>

<span data-ttu-id="37ca3-107">Ha minden felhasználót le szeretne tiltani az 1:1-es hívások rögzítésében, nem kell semmilyen műveletet megtennie.</span><span class="sxs-lookup"><span data-stu-id="37ca3-107">If you prefer to block all users from recording 1:1 calls, you do not need to take any action.</span></span> <span data-ttu-id="37ca3-108">*Az AllowCloudRecordingForCalls* hívásházirend beállítása alapértelmezés szerint $False engedélyezett.</span><span class="sxs-lookup"><span data-stu-id="37ca3-108">*AllowCloudRecordingForCalls* calling policy option will be $False by default.</span></span>

<span data-ttu-id="37ca3-109">Ez a változás az Üzenetközpont következő bejegyzésében található: [(Frissítve) 1:1-es hívásrögzítési](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) házirend – Bevezetés A Teams hívási házirend beállításának beállítását a [Teams PowerShell használatával](https://docs.microsoft.com/microsoftteams/teams-powershell-install)kell beállítani.</span><span class="sxs-lookup"><span data-stu-id="37ca3-109">This change is documented in the following Message Center Post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) To set the Teams Calling Policy Option you must use [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span></span>

<span data-ttu-id="37ca3-110">**A hívásrögzítés engedélyezése 1:1-es hívásokban:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span><span class="sxs-lookup"><span data-stu-id="37ca3-110">**To enable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span></span>

<span data-ttu-id="37ca3-111">**A hívásrögzítés 1:1-es** hívásokban való letiltásához: Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span><span class="sxs-lookup"><span data-stu-id="37ca3-111">**To disable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span></span>

