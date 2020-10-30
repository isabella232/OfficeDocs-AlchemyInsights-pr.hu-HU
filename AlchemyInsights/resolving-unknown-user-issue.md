---
title: Ismeretlen felhasználóval fennálló probléma megoldása a Teams-csevegésben
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003807"
- "6809"
ms.openlocfilehash: 523c11cb9d5c4696703c67c2a6b3184f5d12f8e7
ms.sourcegitcommit: d151b09064df3fb573ae07a387a08d98a9553b9b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807458"
---
# <a name="resolving-issue-with-unknown-user-in-teams-chat"></a><span data-ttu-id="55bfc-102">Az ismeretlen felhasználóval fennálló probléma megoldása a Teams-csevegésben</span><span class="sxs-lookup"><span data-stu-id="55bfc-102">Resolving issue with "Unknown User" in Teams Chat</span></span>

<span data-ttu-id="55bfc-103">Időnként egy eltávolított felhasználó "ismeretlen felhasználó" néven fog megjelenni.</span><span class="sxs-lookup"><span data-stu-id="55bfc-103">At times, a removed user will appear as "Unknown User".</span></span> <span data-ttu-id="55bfc-104">Ez egy [ismert probléma](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/removed-user-appears-as-unknown).</span><span class="sxs-lookup"><span data-stu-id="55bfc-104">This is a [known issue](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/removed-user-appears-as-unknown).</span></span>

<span data-ttu-id="55bfc-105">Ha állandó módon látja a felhasználókat a Teams-csevegésekben "ismeretlen felhasználó" néven, próbálkozzon a gyorsítótárral, és törölje belőle a következőt:</span><span class="sxs-lookup"><span data-stu-id="55bfc-105">If you are persistently seeing users showing as "Unknown User" in Teams chats, try and clear the cache:</span></span>

1.  <span data-ttu-id="55bfc-106">A tálcán kattintson a jobb gombbal a csoportok ikonjára.</span><span class="sxs-lookup"><span data-stu-id="55bfc-106">Right-click the Teams icon in the taskbar.</span></span> <span data-ttu-id="55bfc-107">Kattintson a  **Kilépés** gombra.</span><span class="sxs-lookup"><span data-stu-id="55bfc-107">Click  **Quit** .</span></span>
2.  <span data-ttu-id="55bfc-108">Tallózással keresse meg a számítógépen a%appdata%\Microsoft\teams\ mappát, és törölje az adott könyvtár összes fájlját.</span><span class="sxs-lookup"><span data-stu-id="55bfc-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>

<span data-ttu-id="55bfc-109">Ha meg szeretné akadályozni, hogy a névtelen felhasználók bekapcsolódjanak az értekezletbe, gondoskodjon arról, hogy az előszobában várjon.</span><span class="sxs-lookup"><span data-stu-id="55bfc-109">You can prevent anonymous users from joining meetings by ensuring that they wait in the lobby.</span></span> <span data-ttu-id="55bfc-110">További információért olvassa el [a Teams-értekezlet résztvevőinek beállításainak módosítása](https://support.microsoft.com/office/change-participant-settings-for-a-teams-meeting-53261366-dbd5-45f9-aae9-a70e6354f88e)című témakört.</span><span class="sxs-lookup"><span data-stu-id="55bfc-110">For more information, see [Change participant settings for a Teams meeting](https://support.microsoft.com/office/change-participant-settings-for-a-teams-meeting-53261366-dbd5-45f9-aae9-a70e6354f88e).</span></span>
