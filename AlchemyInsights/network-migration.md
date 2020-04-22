---
title: Hálózati áttelepítés
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "716"
- "6000002"
ms.assetid: b5ab885c-3803-4cc8-adab-94848e226ffb
ms.openlocfilehash: aada8e90d168a4c621dd81ee8d306b934c20d119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43761816"
---
# <a name="network-migration"></a><span data-ttu-id="44886-102">Hálózati áttelepítés</span><span class="sxs-lookup"><span data-stu-id="44886-102">Network Migration</span></span>

<span data-ttu-id="44886-103">Az O365-ös bérlő valószínűleg több Yammer-hálózathoz van társítva egy 1 bérlőben: Sok hálózat konfigurációja.</span><span class="sxs-lookup"><span data-stu-id="44886-103">Your O365 tenant is possibly associated with multiple Yammer networks in a 1 tenant : Many networks configuration.</span></span> <span data-ttu-id="44886-104">2018. október 16-tól a Yammer már nem támogat több, egy bérlőhöz társított Yammer-hálózatot.</span><span class="sxs-lookup"><span data-stu-id="44886-104">Starting October 16, 2018, Yammer will no longer support multiple Yammer networks associated with one tenant.</span></span> <span data-ttu-id="44886-105">A hálózati áttelepítés végrehajtásával az előnyben részesített 1:1 konfigurációt érheti el.</span><span class="sxs-lookup"><span data-stu-id="44886-105">You can perform a Network Migration to get to a preferred 1:1 configuration.</span></span>
  
- <span data-ttu-id="44886-106">A bérlőhöz társított hálózatok listájának megtekintéséhez jelentkezzen be a Yammerbe globális rendszergazdaként, és keresse meg a **Hálózati rendszergazda**, majd a **Hálózati áttelepítés**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="44886-106">To view a list of the networks associated with your tenant, log in to Yammer as an Global Administrator and browse to **Network Admin**, then **Network Migration**.</span></span> <span data-ttu-id="44886-107">Válassza a **Tovább** gombot.</span><span class="sxs-lookup"><span data-stu-id="44886-107">Choose **Next**.</span></span>

- <span data-ttu-id="44886-108">Ha több hálózatot lát a 3-ból 2.</span><span class="sxs-lookup"><span data-stu-id="44886-108">If you see multiple networks listed on Step 2 of 3, then you have multiple Yammer networks associated with your O365 tenant.</span></span>

- <span data-ttu-id="44886-109">Ha 1:1 arányban szeretné kijavítani a konfigurációt, folytassa a Hálózati áttelepítés eszközzel.</span><span class="sxs-lookup"><span data-stu-id="44886-109">To correct your configuration to a 1:1 configuration, continue using the Network Migration tool.</span></span>

- <span data-ttu-id="44886-110">A hálózati áttelepítésről további információt a [Hálózati áttelepítés: Több Yammer-hálózat konszolidálása című témakörben talál.](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)</span><span class="sxs-lookup"><span data-stu-id="44886-110">For more information on Network Migration please see [Network migration: Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>

<span data-ttu-id="44886-111">Felhívjuk:</span><span class="sxs-lookup"><span data-stu-id="44886-111">Please Note:</span></span>
  
- <span data-ttu-id="44886-112">**A hálózati áttelepítés csak az aktív és függőben lévő felhasználókat telepíti át.**</span><span class="sxs-lookup"><span data-stu-id="44886-112">**A network migration migrates only the active and pending users.**</span></span> <span data-ttu-id="44886-113">Az aktív felhasználókkal együtt a felhasználók adatai , például a név és a profilkép is átkerülnek.</span><span class="sxs-lookup"><span data-stu-id="44886-113">Along with the active users, the users' information, such as name and profile picture, is also migrated.</span></span> <span data-ttu-id="44886-114">A hálózati tartalom, beleértve a csoportokat is, nem kerül áttelepítésre.</span><span class="sxs-lookup"><span data-stu-id="44886-114">Any network content, including groups, is not migrated.</span></span>

- <span data-ttu-id="44886-115">**A hálózati áttelepítés nem vonható vissza.**</span><span class="sxs-lookup"><span data-stu-id="44886-115">**Network migration can't be reversed.**</span></span> <span data-ttu-id="44886-116">Az áttelepítés után nem fogja tudni elérni a kiegészítő hálózatot és annak tartalmát.</span><span class="sxs-lookup"><span data-stu-id="44886-116">You will not be able to access your subsidiary network and its content after migration.</span></span> <span data-ttu-id="44886-117">Tehát mielőtt fontolóra veszi a migráció, azt szeretné, hogy gondosan tervezni.</span><span class="sxs-lookup"><span data-stu-id="44886-117">So before you consider a migration, you want to plan carefully.</span></span>
