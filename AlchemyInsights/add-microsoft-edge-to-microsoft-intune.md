---
title: A Microsoft Edge hozzáadása a Microsoft Intune-hoz
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8240"
- "9004604"
ms.openlocfilehash: d56c65910d1c2170d3e0ce9676e913663701db96
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194510"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a><span data-ttu-id="8ca89-102">A Microsoft Edge hozzáadása a Microsoft Intune-hoz</span><span class="sxs-lookup"><span data-stu-id="8ca89-102">Add Microsoft Edge to Microsoft Intune</span></span>

<span data-ttu-id="8ca89-103">A Windows 10 Microsoft Edge telepítésének, konfigurálásának, figyelése és védelme érdekében először hozzá kell adni a Microsoft Intune-hoz.</span><span class="sxs-lookup"><span data-stu-id="8ca89-103">To be able to deploy, configure, monitor, and protect Microsoft Edge for Windows 10, you must first add it to Microsoft Intune.</span></span>

> [!IMPORTANT]
- <span data-ttu-id="8ca89-104">Az Intune támogatja a Microsoft Edge 77-es és újabb verzióit.</span><span class="sxs-lookup"><span data-stu-id="8ca89-104">Intune supports Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="8ca89-105">Az Intune észlelni fogja a Microsoft Edge esetleges meglévő telepített telepítését.</span><span class="sxs-lookup"><span data-stu-id="8ca89-105">Intune will detect any pre-existing installations of Microsoft Edge.</span></span>
- <span data-ttu-id="8ca89-106">Ha a Microsoft Edge felhasználói környezetben van telepítve, a rendszer telepítése felülírja a telepítést a felhasználói környezetben.</span><span class="sxs-lookup"><span data-stu-id="8ca89-106">If Microsoft Edge is installed in user context, a system installation will overwrite the installation in user context.</span></span>
- <span data-ttu-id="8ca89-107">Ha a Microsoft Edge rendszerkörnyezetben van telepítve, a telepítés sikerességéről is beszámolunk.</span><span class="sxs-lookup"><span data-stu-id="8ca89-107">If Microsoft Edge is installed in system context, the installation success will be reported.</span></span>
- <span data-ttu-id="8ca89-108">Az előre telepített Microsoft Edge 77-es és újabb verziók a felhasználói környezetben található összes csatorna esetében felülíródnak a rendszerkörnyezetben telepített Microsoft Edge böngészővel.</span><span class="sxs-lookup"><span data-stu-id="8ca89-108">Pre-installed Microsoft Edge 77 and later versions, for all channels in user context, will be overwritten with Microsoft Edge installed in system context.</span></span>

<span data-ttu-id="8ca89-109">**Előfeltétel**</span><span class="sxs-lookup"><span data-stu-id="8ca89-109">**Prerequisite**</span></span>

<span data-ttu-id="8ca89-110">Windows 10 1709-es vagy újabb verziók</span><span class="sxs-lookup"><span data-stu-id="8ca89-110">Windows 10 version 1709 or later versions</span></span>

<span data-ttu-id="8ca89-111">**A Edge Intune-hoz való hozzáadásának lépései**</span><span class="sxs-lookup"><span data-stu-id="8ca89-111">**Steps to add Edge to Intune**</span></span>

1. <span data-ttu-id="8ca89-112">[Konfigurálja az alkalmazást az Intune-ban.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="8ca89-112">[Configure the app in Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
2. <span data-ttu-id="8ca89-113">[Konfigurálja az app adatait.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="8ca89-113">[Configure the app information](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
3. <span data-ttu-id="8ca89-114">[Adja meg az alkalmazásbeállításokat.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="8ca89-114">[Configure the app settings](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
4. <span data-ttu-id="8ca89-115">[Jelölje ki a keresési tartomány címkéit (nem kötelező).](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="8ca89-115">[Select the scope tags (optional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
5. <span data-ttu-id="8ca89-116">[Adja hozzá az alkalmazást.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="8ca89-116">[Add the app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>

<span data-ttu-id="8ca89-117">További segítségért lásd a [Hibaelhárítás témakört.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="8ca89-117">For more help, see [Troubleshooting](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>




