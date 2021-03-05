---
title: Adatok eltávolítása és eszközök tartalmának törlése az Intune-ból
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416315"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="c5e97-102">Adatok eltávolítása és eszközök tartalmának törlése az Intune-ból</span><span class="sxs-lookup"><span data-stu-id="c5e97-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="c5e97-103">Az Eszköz kivezetése és az Eszköz adatainak törlése távoli művelettel eltávolíthatja az Intune által kezelt céges adatokat, illetve gyári alaphelyzetbe állítást végezhet, és visszaállíthatja az eszköz alapértelmezett beállításait.</span><span class="sxs-lookup"><span data-stu-id="c5e97-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="c5e97-104">Jelentkezzen be a Microsoft 365 Eszközkezelés szolgáltatásba, és válassza az **Eszközök** > **Az összes eszköz** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="c5e97-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="c5e97-105">Válassza ki az eszközt, amelyről törölni szeretné az adatokat.</span><span class="sxs-lookup"><span data-stu-id="c5e97-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="c5e97-106">Válassza ki a végrehajtandó távoli törlés típusát.</span><span class="sxs-lookup"><span data-stu-id="c5e97-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="c5e97-107">A kivezetés csak a szervezeti adatokat törli, míg a teljes törlés visszaállítja az eszköz gyári beállításait.</span><span class="sxs-lookup"><span data-stu-id="c5e97-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="c5e97-108">Az **Igen** gombot választva erősítse meg a műveletet.</span><span class="sxs-lookup"><span data-stu-id="c5e97-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="c5e97-109">A törlés befejeződéséig az Eszközművelet állapota *Megszüntetés függőben* lesz.</span><span class="sxs-lookup"><span data-stu-id="c5e97-109">Until the wipe finishes, the Device action status shows as *Retire Pending*.</span></span>
    <span data-ttu-id="c5e97-110">A művelet befejeződését követően a mobileszköz többé nem lesz látható a felügyelt eszközök listáján.</span><span class="sxs-lookup"><span data-stu-id="c5e97-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

> [!NOTE]
> <span data-ttu-id="c5e97-111">A céges adatok nem távolíthatók el az Azure AD-hez csatlakoztatott eszközökről.</span><span class="sxs-lookup"><span data-stu-id="c5e97-111">Company data can't be removed from devices JOINED to Azure AD.</span></span> 

<span data-ttu-id="c5e97-112">A kivezetési és törlési műveletek hatásairól az alábbi dokumentációban talál részletes tájékoztatást, egyebek között a megőrzött és a törölt adatok ismertetését:</span><span class="sxs-lookup"><span data-stu-id="c5e97-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see following documentation:</span></span>

- <span data-ttu-id="c5e97-113">[Eszközök eltávolítása adattörléssel, kivezetéssel vagy a regisztrációjuk manuális megszüntetésével](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe)</span><span class="sxs-lookup"><span data-stu-id="c5e97-113">[Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span></span>
- [<span data-ttu-id="c5e97-114">Csak a vállalati adatok törlése az Intune által kezelt alkalmazásokból</span><span class="sxs-lookup"><span data-stu-id="c5e97-114">How to wipe only corporate data from Intune-managed apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- <span data-ttu-id="c5e97-115">[Az összes adat törlése macOS rendszerű eszközről](https://docs.microsoft.com/mem/intune/remote-actions/device-erase)</span><span class="sxs-lookup"><span data-stu-id="c5e97-115">[Erase all data from a macOS device](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span></span>