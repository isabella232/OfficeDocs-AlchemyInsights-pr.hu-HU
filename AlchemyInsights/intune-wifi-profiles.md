---
title: Intune Wi-Fi-profilok
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
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555311"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="43cef-102">Intune Wi-Fi-profilok</span><span class="sxs-lookup"><span data-stu-id="43cef-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="43cef-103">Az MDM-ügyfelek Wi-Fi-kapcsolatának sikeres megvalósítása a megfelelően telepített profiltól függ, amely tükrözi a vállalati Wi-Fi infrastruktúra követelményeit.</span><span class="sxs-lookup"><span data-stu-id="43cef-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="43cef-104">A vizsgált ügyfélplatformok megfelelő beállításainak áttekintéséhez lásd:</span><span class="sxs-lookup"><span data-stu-id="43cef-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="43cef-105">Wi-Fi-beállítások hozzáadása a Microsoft Intune-ban Androidot futtató eszközökhöz</span><span class="sxs-lookup"><span data-stu-id="43cef-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="43cef-106">Wi-Fi-beállítások hozzáadása az Android Enterprise dedikált és teljes körűen felügyelt eszközeihez a Microsoft Intune-ban</span><span class="sxs-lookup"><span data-stu-id="43cef-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="43cef-107">Wi-Fi-beállítások hozzáadása iOS- és iPadOS-eszközökhöz a Microsoft Intune-ban</span><span class="sxs-lookup"><span data-stu-id="43cef-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="43cef-108">A Windows 10-es és újabb eszközök Wi-Fi-beállításainak hozzáadása az Intune-ban</span><span class="sxs-lookup"><span data-stu-id="43cef-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="43cef-109">Windows-eszközök Wi-Fi-beállításainak importálása az Intune-ban</span><span class="sxs-lookup"><span data-stu-id="43cef-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="43cef-110">**Gyakori problémák**</span><span class="sxs-lookup"><span data-stu-id="43cef-110">**Common Issues**</span></span>

<span data-ttu-id="43cef-111">**Olyan Wi-Fi-profilt telepítek, amely a Wi-Fi-profilban megadott telepített tanúsítványtól függ. A konfigurációs profilok azonban hibaállapotot mutatnak.**</span><span class="sxs-lookup"><span data-stu-id="43cef-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="43cef-112">Ellenőrizze, hogy az eszköz megkapta-e a tanúsítványt.</span><span class="sxs-lookup"><span data-stu-id="43cef-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="43cef-113">Az Intune-ban nyissa meg a **Minden eszköz lehetőséget,** és válassza ki az eszköz > **eszközkonfigurációját.**</span><span class="sxs-lookup"><span data-stu-id="43cef-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="43cef-114">Ellenőrizze, hogy az összes várt profil szerepel-e a listában, és sikeres állapotban van-e.</span><span class="sxs-lookup"><span data-stu-id="43cef-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="43cef-115">Android-profil esetén, ha köztes tanúsítványláncban van, győződjön meg arról, hogy azok telepítve vannak androidos eszközökre.</span><span class="sxs-lookup"><span data-stu-id="43cef-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="43cef-116">A tanúsítvány állapotának ellenőrzéséhez nyissa meg **az Eszközkonfigurációs**  >  **profilok Android**  >  **köztes hitelesítésszolgáltató**  >  **Properties**  >  **tulajdonságainak megbízható tanúsítványát.**</span><span class="sxs-lookup"><span data-stu-id="43cef-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="43cef-117">Ha továbbra is hibákat lát, tekintse át az eljárásokat és a hibaelhárítási szakaszokat.</span><span class="sxs-lookup"><span data-stu-id="43cef-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="43cef-118">További információt az [SCEP-tanúsítványprofilok Microsoft Intune-nal kapcsolatos hibaelhárításának áttekintése](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="43cef-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="43cef-119">**Wi-Fi profilt telepítettem egy eszközre. Az Intune azt mutatja, hogy sikeres volt, de az eszköz nem csatlakozik a Wi-Fi-hez.**</span><span class="sxs-lookup"><span data-stu-id="43cef-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="43cef-120">A sikeres állapot azt jelenti, hogy az Intune sikeresen telepítette a profilt a konfigurált módon.</span><span class="sxs-lookup"><span data-stu-id="43cef-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="43cef-121">Előfordulhat azonban, hogy ezek a konfigurációk nem felelnek meg a hálózati és/vagy hitelesítési követelményeknek.</span><span class="sxs-lookup"><span data-stu-id="43cef-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="43cef-122">A megkísérelt kapcsolattal kapcsolatos további részletekért tekintse át az infrastruktúra és a hitelesítési szolgáltatás naplóit (a Wi-Fi hozzáférési pont vezérlőn és a hálózati kiszolgáló/sugár kiszolgálón).</span><span class="sxs-lookup"><span data-stu-id="43cef-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="43cef-123">Előfordulhat, hogy a naplók összegyűjtéséhez és áttekintéséhez együtt kell működnie a hálózati infrastruktúra csapatával vagy a külső Wi-Fi-szolgáltatóval.</span><span class="sxs-lookup"><span data-stu-id="43cef-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>