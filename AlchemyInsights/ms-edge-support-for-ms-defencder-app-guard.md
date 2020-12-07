---
title: Microsoft Edge támogatása a Microsoft Defender alkalmazás-Gárda számára
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583582"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a><span data-ttu-id="fcd06-102">Microsoft Edge támogatása a Microsoft Defender alkalmazás-Gárda számára</span><span class="sxs-lookup"><span data-stu-id="fcd06-102">Microsoft Edge's support for Microsoft Defender Application Guard</span></span>

<span data-ttu-id="fcd06-103">A Windows 10 és a Microsoft Edge rendszerhez készült alkalmazás-őr hardveres elkülönítési megközelítést használ, amely lehetővé teszi, hogy egy felhasználó egy nem védett webhelyre navigáljon egy elszigetelt, hiper-V-os tárolótól, amely a fogadó operációs rendszertől elválasztva van.</span><span class="sxs-lookup"><span data-stu-id="fcd06-103">Designed for Windows 10 and Microsoft Edge, Application Guard uses a hardware-isolation approach that lets a user navigate an untrusted site from inside an isolated, Hyper-V–enabled container, separated from the host operating system.</span></span>

<span data-ttu-id="fcd06-104">A vállalati rendszergazdák a megbízható webhelyek, a felhőalapú erőforrások és a belső hálózatok listáját határozzák meg.</span><span class="sxs-lookup"><span data-stu-id="fcd06-104">An enterprise admin defines a list of trusted websites, cloud resources, and internal networks.</span></span> <span data-ttu-id="fcd06-105">Ha egy felhasználó olyan webhelyet látogat meg, amely nem szerepel a listán, a Microsoft Edge megnyitja a webhelyet a tárolóban.</span><span class="sxs-lookup"><span data-stu-id="fcd06-105">When a user visits a site that's not on the list, Microsoft Edge will open the site in the container.</span></span> <span data-ttu-id="fcd06-106">Ez azt jelenti, hogy ha a webhely kártékonynak tűnik, a gazdaszámítógép védett marad, és a támadó nem fog megjelenni a vállalati adatszolgáltatásban.</span><span class="sxs-lookup"><span data-stu-id="fcd06-106">This means that if the site turns out to be malicious, the host PC will remain protected and the attacker won't get to the enterprise data.</span></span>

<span data-ttu-id="fcd06-107">A bővítmények telepítése a tárolóban a Microsoft Edge 81-es verziójában érhető el, és egy házirenden keresztül is ellenőrizhető.</span><span class="sxs-lookup"><span data-stu-id="fcd06-107">Installation of extensions in the container is supported as of Microsoft Edge version 81, and it can be controlled via a policy.</span></span> <span data-ttu-id="fcd06-108">Az ExtensionInstallForcelist-házirendben használt updateURL-címet semleges erőforrásként kell hozzáadni az alkalmazás-Gárda által használt hálózat-elkülönítési házirendekhez.</span><span class="sxs-lookup"><span data-stu-id="fcd06-108">The updateURL address that gets used in the ExtensionInstallForcelist policy should be added as a Neutral Resource in the Network Isolation policies used by Application Guard.</span></span>

<span data-ttu-id="fcd06-109">További információt a Microsoft [Edge támogatása a Microsoft Defender alkalmazás-Gárda számára](https://go.microsoft.com/fwlink/?linkid=2134229)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="fcd06-109">For more info, see [Microsoft Edge support for Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span></span>
