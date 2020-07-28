---
title: Adatok eltávolítása és eszközök törlése az Intune-ból
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439648"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="54052-102">Adatok eltávolítása és eszközök törlése az Intune-ból</span><span class="sxs-lookup"><span data-stu-id="54052-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="54052-103">Az Eszköz kivonása és az Eszköztörlés távoli műveletek segítségével eltávolíthatja az Intune által kezelt vállalati adatokat, vagy gyári alaphelyzetbe állításra, és visszaállíthatja az eszközt az alapértelmezett beállításokra.</span><span class="sxs-lookup"><span data-stu-id="54052-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="54052-104">Jelentkezzen be a Microsoft 365 Eszközkezelés szolgáltatásba, és nyissa meg **az Eszközök**minden  >  **eszköz lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="54052-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="54052-105">Jelölje ki a törölni kívánt eszközt.</span><span class="sxs-lookup"><span data-stu-id="54052-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="54052-106">Válassza ki a tenni kívánt távoli törlés típusát.</span><span class="sxs-lookup"><span data-stu-id="54052-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="54052-107">A kivonás csak a szervezeti adatokat törli, míg a teljes törlés visszaállítja az eszközt a gyári beállításokra.</span><span class="sxs-lookup"><span data-stu-id="54052-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="54052-108">A megerősítéshez válassza az **Igen** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="54052-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="54052-109">Amíg a törlés be nem fejeződik, az Eszköz művelet állapota állapot a Függőben állapot befejezése.</span><span class="sxs-lookup"><span data-stu-id="54052-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="54052-110">A művelet befejezése után a továbbiakban nem jelenik meg a mobileszköz a felügyelt eszközök listájában.</span><span class="sxs-lookup"><span data-stu-id="54052-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="54052-111">**Megjegyzés:** A vállalati adatok nem távolíthatók el az Azure AD-hez csatlakozott eszközökről.</span><span class="sxs-lookup"><span data-stu-id="54052-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="54052-112">A Kivonásés és törlés műveletek hatásának részletes megtekintéséről, beleértve a megőrzött és a törölt műveleteket, olvassa el [az Eszközök eltávolítása törléssel, kivonással vagy manuálisan történő unrerollingozással című témakört.](https://docs.microsoft.com/intune/devices-wipe)</span><span class="sxs-lookup"><span data-stu-id="54052-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="54052-113">Az összes adat macOS-eszközről történő törléséről az [Összes adat törlése macOS-eszközről .to](https://docs.microsoft.com/intune/device-erase)erase all data from a macOS device to erase all data from a macOS device to erase all data from a macOS device to</span><span class="sxs-lookup"><span data-stu-id="54052-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>