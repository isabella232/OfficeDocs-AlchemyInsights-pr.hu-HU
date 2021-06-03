---
title: A endpoint DLP not deployed to user's device
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731586"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a><span data-ttu-id="f3769-102">A endpoint DLP not deployed to user's device</span><span class="sxs-lookup"><span data-stu-id="f3769-102">Endpoint DLP not deployed to user's device</span></span>

<span data-ttu-id="f3769-103">Ha a Végpontok adatveszteség-megelőzés (DLP) beállítás nem vonatkozik egy felhasználó eszközére, ellenőrizze, hogy megfelel-e az alábbi követelményeknek:</span><span class="sxs-lookup"><span data-stu-id="f3769-103">If the Endpoint data loss prevention (DLP) setting has not applied to a user's device, confirm you meet these requirements:</span></span>

- <span data-ttu-id="f3769-104">Windows 10 x64-es build 1809-es vagy újabb build telepítve van az eszközön.</span><span class="sxs-lookup"><span data-stu-id="f3769-104">Windows 10 x64 build 1809 or later is installed on the device.</span></span>
- <span data-ttu-id="f3769-105">A kártevők elleni ügyfélprogram 4.18.2009.7-es vagy újabb verziója telepítve van.</span><span class="sxs-lookup"><span data-stu-id="f3769-105">Anti-malware client version 4.18.2009.7 or later is installed.</span></span>
- <span data-ttu-id="f3769-106">Az eszköz **az alábbi** eszközök egyike:</span><span class="sxs-lookup"><span data-stu-id="f3769-106">The device is **one** of these:</span></span>
    
    - <span data-ttu-id="f3769-107">Azure Active Directory (Azure AD) csatlakozva</span><span class="sxs-lookup"><span data-stu-id="f3769-107">Azure Active Directory (Azure AD) joined</span></span>
    - <span data-ttu-id="f3769-108">Hibrid Azure AD-csatlakozás</span><span class="sxs-lookup"><span data-stu-id="f3769-108">Hybrid Azure AD joined</span></span>
    - <span data-ttu-id="f3769-109">AAD regisztrálva</span><span class="sxs-lookup"><span data-stu-id="f3769-109">AAD registered</span></span>

- <span data-ttu-id="f3769-110">A házirendműveletek érvénybe lépésekhez győződjön meg arról, Chromium microsoft Chromium Edge böngésző telepítve van a végponteszközre.</span><span class="sxs-lookup"><span data-stu-id="f3769-110">To enforce policy actions, make sure Microsoft Chromium Edge browser is installed on the endpoint device.</span></span>

<span data-ttu-id="f3769-111">Az Endpoint DLP üzembe helyezésének további követelményeiről az Első lépések [az végpontok adatveszteség-megelőzési szolgáltatásával .](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)</span><span class="sxs-lookup"><span data-stu-id="f3769-111">For additional requirements for deploying Endpoint DLP, see [Get started with Endpoint data loss prevention](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).</span></span>