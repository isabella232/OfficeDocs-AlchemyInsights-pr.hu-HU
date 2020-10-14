---
title: Intune win32 app-telepítő
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461870"
---
# <a name="intune-win32-app-deployment"></a><span data-ttu-id="0c3c0-102">Intune win32 app-telepítő</span><span class="sxs-lookup"><span data-stu-id="0c3c0-102">Intune Win32 app deployment</span></span>

<span data-ttu-id="0c3c0-103">A Microsoft Intune lehetővé teszi a Win32-alkalmazásokat, például az MSI-t és az Office-t. Az EXE-fájlt Windows 10-es eszközökre kell telepíteni.</span><span class="sxs-lookup"><span data-stu-id="0c3c0-103">Microsoft Intune allows Win32 applications, including but not limited to MSI and .EXE’s to be deployed to Windows 10 devices.</span></span> <span data-ttu-id="0c3c0-104">A használt központi telepítési mechanizmushoz az Intune felügyeleti bővítmény (IME) szükséges a céleszköz megadásához.</span><span class="sxs-lookup"><span data-stu-id="0c3c0-104">The deployment mechanism used requires the Intune Management Extension (IME) to be present on the target device.</span></span> <span data-ttu-id="0c3c0-105">Az ÍRÁSJEGYBEVIVŐt automatikusan telepíti a rendszer a PowerShell-parancsfájlok vagy a Win32-alkalmazások felhasználóhoz vagy eszközhöz való telepítésének eredményeképpen.</span><span class="sxs-lookup"><span data-stu-id="0c3c0-105">The IME will be installed automatically as a result of targeting a powershell script or win32 application deployment to a user / device.</span></span>

<span data-ttu-id="0c3c0-106">Vannak olyan előfeltételek is, amelyeknek teljesíteniük kell a Win32 alkalmazások központi telepítéséhez, amelyek a következők:</span><span class="sxs-lookup"><span data-stu-id="0c3c0-106">There are also a set of pre-requisites which must be met in order to deploy Win32 apps which include:</span></span>

- <span data-ttu-id="0c3c0-107">Támogatott platformok: a Windows 10 1607-es vagy újabb verziója (nagyvállalati, Pro-és oktatási verzió).</span><span class="sxs-lookup"><span data-stu-id="0c3c0-107">Supported platforms: Windows 10 version 1607 or later (Enterprise, Pro, and Education versions).</span></span>
- <span data-ttu-id="0c3c0-108">Támogatott architektúra: x86 és x64.</span><span class="sxs-lookup"><span data-stu-id="0c3c0-108">Supported architecture: x86 and x64.</span></span>
- <span data-ttu-id="0c3c0-109">Eszközkezelés: a AAD csatlakozott és automatikusan regisztrált (többek között a hibrid tartomány csatlakozott és a csoportházirend automatikus igénylése).</span><span class="sxs-lookup"><span data-stu-id="0c3c0-109">Device Management: AAD joined and auto-enrolled (including hybrid domain joined and group policy auto-enrolled).</span></span>
- <span data-ttu-id="0c3c0-110">Alkalmazásspecifikus csomag formátuma:. a [Microsoft Win32 Content PREP Tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare)által készített **intunewin** -fájl</span><span class="sxs-lookup"><span data-stu-id="0c3c0-110">Application Package format: .**intunewin**  file prepared by the [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span></span>
- <span data-ttu-id="0c3c0-111">Korlátozások</span><span class="sxs-lookup"><span data-stu-id="0c3c0-111">Limitations:</span></span>
    - <span data-ttu-id="0c3c0-112">Maximális méret: 8GB.</span><span class="sxs-lookup"><span data-stu-id="0c3c0-112">Maximum size: 8GB.</span></span>
    - <span data-ttu-id="0c3c0-113">Nem támogatott architektúra: karok.</span><span class="sxs-lookup"><span data-stu-id="0c3c0-113">Unsupported architecture: ARMs.</span></span>

<span data-ttu-id="0c3c0-114">A fenti lépésekkel kapcsolatos további tudnivalókért olvassa el a[Win32-alkalmazás hozzáadása, hozzárendelése és figyelése a Microsoft Intune-ban](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)című témakört.</span><span class="sxs-lookup"><span data-stu-id="0c3c0-114">Review the doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for information related to those steps.</span></span>

<span data-ttu-id="0c3c0-115">A Windows és a Win32 alkalmazások hibaelhárítási alkalmazásainak ismertetése a következő dokumentumokban olvasható.</span><span class="sxs-lookup"><span data-stu-id="0c3c0-115">Details on troubleshooting application deployment on Windows including Win32 apps can be reviewed in the following documents</span></span>

- [<span data-ttu-id="0c3c0-116">Az alkalmazások telepítésével kapcsolatos hibák elhárítása</span><span class="sxs-lookup"><span data-stu-id="0c3c0-116">Troubleshoot App Installation issues</span></span>](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [<span data-ttu-id="0c3c0-117">Win32-alkalmazások – hibaelhárítás</span><span class="sxs-lookup"><span data-stu-id="0c3c0-117">Troubleshoot Win32 Apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)