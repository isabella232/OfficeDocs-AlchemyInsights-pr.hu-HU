---
title: Hálózati áttelepítés
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "716"
- "6000002"
ms.assetid: b5ab885c-3803-4cc8-adab-94848e226ffb
ms.openlocfilehash: 6f026f932bb35d12d32ce7eddf49e49a44db7f31
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799566"
---
# <a name="network-migration"></a><span data-ttu-id="e798b-102">Hálózati áttelepítés</span><span class="sxs-lookup"><span data-stu-id="e798b-102">Network Migration</span></span>

<span data-ttu-id="e798b-103">Az O365-bérlői fiókja valószínűleg több Yammer-hálózattal van társítva egy 1 bérlői fiókban: számos hálózati konfigurációt.</span><span class="sxs-lookup"><span data-stu-id="e798b-103">Your O365 tenant is possibly associated with multiple Yammer networks in a 1 tenant : Many networks configuration.</span></span> <span data-ttu-id="e798b-104">Az 2018 október 16-án kezdődően a Yammer többé nem támogatja az egyik bérlőhöz társított több Yammer-hálózatot.</span><span class="sxs-lookup"><span data-stu-id="e798b-104">Starting October 16, 2018, Yammer will no longer support multiple Yammer networks associated with one tenant.</span></span> <span data-ttu-id="e798b-105">A hálózati áttelepítés segítségével elérheti a kívánt 1:1-konfigurációt.</span><span class="sxs-lookup"><span data-stu-id="e798b-105">You can perform a Network Migration to get to a preferred 1:1 configuration.</span></span>
  
- <span data-ttu-id="e798b-106">Ha meg szeretné tekinteni a bérlői webhelyekkel társított hálózatok listáját, jelentkezzen be az Yammer-be globális rendszergazdaként, és keresse meg a **hálózati rendszergazda**, majd a **hálózat áttelepítése**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="e798b-106">To view a list of the networks associated with your tenant, log in to Yammer as an Global Administrator and browse to **Network Admin**, then **Network Migration**.</span></span> <span data-ttu-id="e798b-107">Válassza a **Tovább** gombot.</span><span class="sxs-lookup"><span data-stu-id="e798b-107">Choose **Next**.</span></span>

- <span data-ttu-id="e798b-108">Ha a 3 lépésen belül több hálózatot is lát, akkor több Yammer-hálózat van társítva a O365-bérlői webhelyhez.</span><span class="sxs-lookup"><span data-stu-id="e798b-108">If you see multiple networks listed on Step 2 of 3, then you have multiple Yammer networks associated with your O365 tenant.</span></span>

- <span data-ttu-id="e798b-109">Ha a konfigurációt egy 1:1-konfigurációra szeretné korrigálni, folytassa a hálózati áttelepítési eszköz használatát.</span><span class="sxs-lookup"><span data-stu-id="e798b-109">To correct your configuration to a 1:1 configuration, continue using the Network Migration tool.</span></span>

- <span data-ttu-id="e798b-110">A hálózat áttelepítéséről további információt a [hálózati áttelepítés: több Yammer-hálózat összevonása](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="e798b-110">For more information on Network Migration please see [Network migration: Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>

<span data-ttu-id="e798b-111">Kérjük, vegye figyelembe az alábbiakat:</span><span class="sxs-lookup"><span data-stu-id="e798b-111">Please Note:</span></span>
  
- <span data-ttu-id="e798b-112">**A hálózati áttelepítés csak az aktív és a függőben lévő felhasználókat telepíti át.**</span><span class="sxs-lookup"><span data-stu-id="e798b-112">**A network migration migrates only the active and pending users.**</span></span> <span data-ttu-id="e798b-113">Az aktív felhasználókkal együtt a felhasználók adatai, például a név és a profil képe is át van telepítve.</span><span class="sxs-lookup"><span data-stu-id="e798b-113">Along with the active users, the users' information, such as name and profile picture, is also migrated.</span></span> <span data-ttu-id="e798b-114">Bármely hálózati tartalom, többek között a csoportok nem települnek át.</span><span class="sxs-lookup"><span data-stu-id="e798b-114">Any network content, including groups, is not migrated.</span></span>

- <span data-ttu-id="e798b-115">**A hálózati áttelepítést nem lehet visszafordítani.**</span><span class="sxs-lookup"><span data-stu-id="e798b-115">**Network migration can't be reversed.**</span></span> <span data-ttu-id="e798b-116">Az áttelepítés után nem fog tudni hozzáférni a kisegítő hálózathoz és annak tartalmához.</span><span class="sxs-lookup"><span data-stu-id="e798b-116">You will not be able to access your subsidiary network and its content after migration.</span></span> <span data-ttu-id="e798b-117">Az áttelepítés előtt érdemes megtervezni az áttelepítést.</span><span class="sxs-lookup"><span data-stu-id="e798b-117">So before you consider a migration, you want to plan carefully.</span></span>
