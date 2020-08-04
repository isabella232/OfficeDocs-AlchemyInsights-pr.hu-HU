---
title: VPN-rel kapcsolatos problémák
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
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555236"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="09790-102">VPN-rel kapcsolatos problémák</span><span class="sxs-lookup"><span data-stu-id="09790-102">VPN related issues</span></span>

<span data-ttu-id="09790-103">Az MDM-ügyfelek VPN-kapcsolatának sikeres megvalósítása olyan üzembe helyezett profiltól függ, amely megfelelően tükrözi a VPN-infrastruktúra követelményeit.</span><span class="sxs-lookup"><span data-stu-id="09790-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="09790-104">A vizsgált ügyfélplatformok megfelelő beállításairól az:</span><span class="sxs-lookup"><span data-stu-id="09790-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="09790-105">A Windows 10 és a Windows holografikus eszköz beállításai a VPN-kapcsolatok hozzáadásához az Intune-nal</span><span class="sxs-lookup"><span data-stu-id="09790-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="09790-106">VPN-beállítások hozzáadása iOS- és iPadOS-eszközökön a Microsoft Intune-ban</span><span class="sxs-lookup"><span data-stu-id="09790-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="09790-107">Az Android-eszköz beállításai a VPN in Intune-ban való konfigurálásához</span><span class="sxs-lookup"><span data-stu-id="09790-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="09790-108">VPN-beállítások hozzáadása macOS-eszközökön a Microsoft Intune-ban</span><span class="sxs-lookup"><span data-stu-id="09790-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="09790-109">Ha a VPN-profil tanúsítványalapú hitelesítést használ, győződjön meg arról, hogy a VPN-profilhoz kapcsolt főtanúsítvány- és ügyfélhitelesítési tanúsítványprofilok telepítése sikeresen megtörtént.</span><span class="sxs-lookup"><span data-stu-id="09790-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="09790-110">**Gyakori problémák**</span><span class="sxs-lookup"><span data-stu-id="09790-110">**Common Issues**</span></span>

<span data-ttu-id="09790-111">**Vpn-profilt telepítettem egy eszközre. Az Intune azt mutatja, hogy sikeres volt, de az eszköz nem csatlakozik a VPN-hez.**</span><span class="sxs-lookup"><span data-stu-id="09790-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="09790-112">A sikeres állapot azt jelenti, hogy az Intune sikeresen telepítette a profilt a konfigurált módon.</span><span class="sxs-lookup"><span data-stu-id="09790-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="09790-113">Előfordulhat azonban, hogy ezek a konfigurációk nem felelnek meg a hálózati és/vagy hitelesítési követelményeknek.</span><span class="sxs-lookup"><span data-stu-id="09790-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="09790-114">Tekintse át az infrastruktúra és a hitelesítési szolgáltatás naplóit (a VPN-kiszolgálón és a nps/radius-kiszolgálón) a megkísérelt kapcsolattal kapcsolatos további részletekért.</span><span class="sxs-lookup"><span data-stu-id="09790-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="09790-115">Előfordulhat, hogy a naplók összegyűjtéséhez és áttekintéséhez együtt kell működnie a hálózati infrastruktúra csapatával vagy a külső VPN-szállítóval.</span><span class="sxs-lookup"><span data-stu-id="09790-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="09790-116">**Amikor egyéni VPN-t konfigurálok iOS-hez, az alkalmazásonkénti VPN-funkció nem lesz elérhető.**</span><span class="sxs-lookup"><span data-stu-id="09790-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="09790-117">Az Intune-ban az iOS-eszközökhöz való alkalmazásonkénti VPN jelenleg elérhető a szolgáltatók és partnerek egy adott listája számára, akiknek szintén meg kell felelniük a tanúsítvány előfeltételeinek, mielőtt alkalmazásonkénti VPN-t konfigurálnának.</span><span class="sxs-lookup"><span data-stu-id="09790-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="09790-118">További információ: [Az alkalmazásonkénti virtuális magánhálózat (VPN) beállítása iOS/iPadOS eszközökhöz az Intune-ban.](https://docs.microsoft.com/intune/vpn-setting-configure-per-app)</span><span class="sxs-lookup"><span data-stu-id="09790-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="09790-119">Az Intune összes VPN-kapcsolattípusáról további információt az [Intune VPN-kiszolgálóihoz való csatlakozáshoz vpn-profilok létrehozása című témakörben talál.](https://docs.microsoft.com/intune/vpn-settings-configure)</span><span class="sxs-lookup"><span data-stu-id="09790-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="09790-120">**Az iOS igény szerinti VPN-je nem aktiválódik, ha egy konfigurált tartományhoz hozzáfér**</span><span class="sxs-lookup"><span data-stu-id="09790-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="09790-121">Az automatikus VPN-beállítások teszteléséhez állítsa be a következő értékeket:</span><span class="sxs-lookup"><span data-stu-id="09790-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="09790-122">A következőt szeretném **tenni: Minden csatlakozási kísérlet kiértékelése**</span><span class="sxs-lookup"><span data-stu-id="09790-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="09790-123">Válassza ki, hogy csatlakozik-e: **Csatlakozás, ha szükséges**</span><span class="sxs-lookup"><span data-stu-id="09790-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="09790-124">Amikor a felhasználók hozzáférnek ezekhez a tartományokhoz: **céltartomány** *név*</span><span class="sxs-lookup"><span data-stu-id="09790-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="09790-125">Ha a fenti konfiguráció nem sikerült, adja hozzá a következő elemet:</span><span class="sxs-lookup"><span data-stu-id="09790-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="09790-126">Ha ez az URL nem érhető el, kényszerítse a VPN-t: **BADURL**</span><span class="sxs-lookup"><span data-stu-id="09790-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>