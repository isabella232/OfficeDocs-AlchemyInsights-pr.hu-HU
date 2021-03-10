---
title: Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693815"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="f9c8d-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span><span class="sxs-lookup"><span data-stu-id="f9c8d-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="f9c8d-103">Ezt a következőképpen teheti meg:</span><span class="sxs-lookup"><span data-stu-id="f9c8d-103">Here's how:</span></span>

1. <span data-ttu-id="f9c8d-104">A harmadik féltől származó megoldás Microsoft Defender ATP-ről való leválasztása érdekében kövesse a külső gyártó dokumentációját.</span><span class="sxs-lookup"><span data-stu-id="f9c8d-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="f9c8d-105">Az Azure Active Directory-bérlőből távolítsa el a külső megoldás engedélyét:</span><span class="sxs-lookup"><span data-stu-id="f9c8d-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="f9c8d-106">Jelentkezzen be az [Azure Portalba.](https://go.microsoft.com/fwlink/?linkid=2125612)</span><span class="sxs-lookup"><span data-stu-id="f9c8d-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="f9c8d-107">Válassza **az Azure** Active Directory Enterprise Applications összes  >    >  **szolgáltatását.**</span><span class="sxs-lookup"><span data-stu-id="f9c8d-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="f9c8d-108">Jelölje ki azt az alkalmazást, amelyről ki szeretné választani a táblát.</span><span class="sxs-lookup"><span data-stu-id="f9c8d-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="f9c8d-109">Válassza a **Törlés gombot.**</span><span class="sxs-lookup"><span data-stu-id="f9c8d-109">Select **Delete**.</span></span>

<span data-ttu-id="f9c8d-110">További információért olvassa el a nem Windows rendszerű eszközök [kitáblás eszközeit.](https://go.microsoft.com/fwlink/?linkid=2143630)</span><span class="sxs-lookup"><span data-stu-id="f9c8d-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
