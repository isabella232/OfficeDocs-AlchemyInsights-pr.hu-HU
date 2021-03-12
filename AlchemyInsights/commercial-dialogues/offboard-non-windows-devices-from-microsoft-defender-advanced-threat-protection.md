---
title: Nem Windows rendszerű eszközök kitáblája a Microsoft Defender Komplex veszélyforrások elleni védelem (ATP) alkalmazásból
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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745647"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="e5c43-102">Nem Windows rendszerű eszközök kitáblája a Microsoft Defender Komplex veszélyforrások elleni védelem (ATP) alkalmazásból</span><span class="sxs-lookup"><span data-stu-id="e5c43-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="e5c43-103">Ezt a következőképpen teheti meg:</span><span class="sxs-lookup"><span data-stu-id="e5c43-103">Here's how:</span></span>

1. <span data-ttu-id="e5c43-104">A harmadik féltől származó megoldás Microsoft Defender ATP-től való leválasztása érdekében kövesse a külső gyártó dokumentációját.</span><span class="sxs-lookup"><span data-stu-id="e5c43-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="e5c43-105">Az Azure Active Directory bérlői webhelyről távolítsa el a külső megoldás engedélyét:</span><span class="sxs-lookup"><span data-stu-id="e5c43-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="e5c43-106">Jelentkezzen be az [Azure Portalba.](https://go.microsoft.com/fwlink/?linkid=2125612)</span><span class="sxs-lookup"><span data-stu-id="e5c43-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="e5c43-107">Válassza **a Minden**  >  **szolgáltatás: Azure Active Directory**  >  **Nagyvállalati alkalmazások lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="e5c43-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="e5c43-108">Jelölje ki azt az alkalmazást, amelyről ki szeretné választani a táblát.</span><span class="sxs-lookup"><span data-stu-id="e5c43-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="e5c43-109">Válassza a **Törlés gombot.**</span><span class="sxs-lookup"><span data-stu-id="e5c43-109">Select **Delete**.</span></span>

<span data-ttu-id="e5c43-110">További információért olvassa el a Nem Windows rendszerű eszközök [ki vannak kapcsolva.](https://go.microsoft.com/fwlink/?linkid=2143630)</span><span class="sxs-lookup"><span data-stu-id="e5c43-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
