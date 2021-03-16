---
title: A Microsoft Search háttérszolgáltatásának eltávolítása a Bingben
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816201"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a><span data-ttu-id="294cb-102">A Microsoft Search háttérszolgáltatásának eltávolítása a Bingben</span><span class="sxs-lookup"><span data-stu-id="294cb-102">Remove the background service for Microsoft Search in Bing</span></span>

<span data-ttu-id="294cb-103">Ha el szeretné távolítani a Microsoft Search háttérszolgáltatását a Bingben, próbálkozzon az alábbi megoldásokkal:</span><span class="sxs-lookup"><span data-stu-id="294cb-103">To remove the background service for Microsoft Search in Bing, you can try the following remedies:</span></span>

1. <span data-ttu-id="294cb-104">Az eredeti keresőmotor-beállításokhoz való visszatéréshez tegye a következőket:</span><span class="sxs-lookup"><span data-stu-id="294cb-104">To revert to the original search engine settings, do the following things:</span></span>

    <span data-ttu-id="294cb-105">a.</span><span class="sxs-lookup"><span data-stu-id="294cb-105">a.</span></span> <span data-ttu-id="294cb-106">Kapcsolja ki a Bing használata alapértelmezett keresőmotorként **kapcsolót. [](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome)**</span><span class="sxs-lookup"><span data-stu-id="294cb-106">Switch the **Use Bing as your default search engine [toggle](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Off**.</span></span>

    <span data-ttu-id="294cb-107">b.</span><span class="sxs-lookup"><span data-stu-id="294cb-107">b.</span></span> <span data-ttu-id="294cb-108">[A Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) Felügyeleti központban törölje a szervezet minden felhasználóját érintő beállítást.</span><span class="sxs-lookup"><span data-stu-id="294cb-108">[Go to the Microsoft 365 admin center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) and clear the setting that affects all users in your organization.</span></span>

2. <span data-ttu-id="294cb-109">Ha el szeretné távolítani a háttérszolgáltatást egy adott eszközről, tegye a következőket:</span><span class="sxs-lookup"><span data-stu-id="294cb-109">To remove the background service from an individual device, do the following tasks:</span></span>

    <span data-ttu-id="294cb-110">a.</span><span class="sxs-lookup"><span data-stu-id="294cb-110">a.</span></span> <span data-ttu-id="294cb-111">Válassza **a Vezérlőpult > Programok > szolgáltatások lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="294cb-111">Choose **Control Panel > Programs > Programs and Features**.</span></span>

    <span data-ttu-id="294cb-112">b.</span><span class="sxs-lookup"><span data-stu-id="294cb-112">b.</span></span> <span data-ttu-id="294cb-113">Kattintson a jobb **gombbal a Microsoft Search elemre** a Bingben a telepített programok listája alatt, és kattintson az Eltávolítás **parancsra.**</span><span class="sxs-lookup"><span data-stu-id="294cb-113">Right-click **Microsoft Search in Bing** under the list of installed programs, and then click **Uninstall**.</span></span>

3. <span data-ttu-id="294cb-114">Ha a háttérszolgáltatást több eszközről szeretné eltávolítani a szervezetből, jelentkezzen be rendszergazdaként, és futtassa az alábbi parancsot egy parancsfájlban:</span><span class="sxs-lookup"><span data-stu-id="294cb-114">To remove the background service from multiple devices in your organization, log in as an administrator and run the following command in a script:</span></span> 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
