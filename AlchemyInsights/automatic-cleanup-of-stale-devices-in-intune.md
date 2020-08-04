---
title: Az elavult eszközök automatikus karbantartása az Intune-ban
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555221"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="15a20-102">Az elavult eszközök automatikus karbantartása az Intune-ban</span><span class="sxs-lookup"><span data-stu-id="15a20-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="15a20-103">Az Intune lehetővé teszi a rendszergazda számára, hogy 90 és 270 nap közötti időintervallumot konfiguráljon, amely után az elavult eszközöket eltávolítja a szolgáltatásból.</span><span class="sxs-lookup"><span data-stu-id="15a20-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="15a20-104">Ez a beállítás szervezeti szintű, és az aktiválás után azonnal életbe lép.</span><span class="sxs-lookup"><span data-stu-id="15a20-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="15a20-105">A beállításnál hosszabb ideig az Intune-kiszolgálón nem bejelentkezett eszközök véglegesen törlődnek.</span><span class="sxs-lookup"><span data-stu-id="15a20-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="15a20-106">**Megjegyzés:** Csak az MDM-eszközobjektumok jogosultak erre a törlési műveletre.</span><span class="sxs-lookup"><span data-stu-id="15a20-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="15a20-107">Csak az EAS-eszközobjektumok nem tartoznak ide.</span><span class="sxs-lookup"><span data-stu-id="15a20-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="15a20-108">További információ arról, hogy egy eszköz mikor válik jogosulttá a törlésre az eszköz tisztítási beállítása és "állapota" alapján:</span><span class="sxs-lookup"><span data-stu-id="15a20-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="15a20-109">Beállítás: **Eszközök törlése az utolsó bejelentkezés idáig: Igen (néhány érték (N) a megadott napokban)**</span><span class="sxs-lookup"><span data-stu-id="15a20-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="15a20-110">A beállításban beállított érték (N) alapján az Intune szolgáltatás törli az eszközt a megadott napokban, miután utoljára sikeresen bejelentkezett.</span><span class="sxs-lookup"><span data-stu-id="15a20-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="15a20-111">Beállítás: **Eszközök törlése az utolsó bejelentkezés idáig: Nem**</span><span class="sxs-lookup"><span data-stu-id="15a20-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="15a20-112">180 nappal az eszköztanúsítvány lejárta után, és nem újul meg, az eszköz törlődik.</span><span class="sxs-lookup"><span data-stu-id="15a20-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="15a20-113">**Megjegyzés:** Mindkét esetben az eszközt sikeresen regisztrálni kell az Intune-ban.</span><span class="sxs-lookup"><span data-stu-id="15a20-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="15a20-114">A regisztráció az Intune szolgáltatással való első eszköz-bejelentkezés során történik.</span><span class="sxs-lookup"><span data-stu-id="15a20-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="15a20-115">Ha egy eszköz sikeresen regisztrál az Intune-ra, de nem lesz Regisztrálva az Intune-ban, az eszköz a regisztráció után 270 nappal törlődik.</span><span class="sxs-lookup"><span data-stu-id="15a20-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="15a20-116">(90 nap az eszköz visszavontként való megjelölésére, majd további 180 nap a rekord törlésére.)</span><span class="sxs-lookup"><span data-stu-id="15a20-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="15a20-117">Jelenleg nincs olyan mechanizmus az Intune konzolon, amely egy adott eszköz eszközminősítésének lejárati dátumát állapítana meg.</span><span class="sxs-lookup"><span data-stu-id="15a20-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>