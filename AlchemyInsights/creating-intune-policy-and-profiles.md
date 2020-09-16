---
title: Intune-házirendek és-profilok létrehozása
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1064"
- "6700005"
ms.openlocfilehash: 9026beac824ebc3849241dbb534c27b00ef1d0eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47746761"
---
# <a name="creating-intune-policy-and-profiles"></a><span data-ttu-id="ce986-102">Intune-házirendek és-profilok létrehozása</span><span class="sxs-lookup"><span data-stu-id="ce986-102">Creating Intune policy and profiles</span></span>

<span data-ttu-id="ce986-103">Az Intune-ban különböző dolgokat tartalmazó házirendeket és profilokat hozhat létre.</span><span class="sxs-lookup"><span data-stu-id="ce986-103">In Intune, you can create policies and profiles that do different things.</span></span>

- <span data-ttu-id="ce986-104">**Beiratkozási profilok**: az eszközök platformon való előre beállítása, a felhasználói affinitás engedélyezése, többtényezős hitelesítés használata stb.</span><span class="sxs-lookup"><span data-stu-id="ce986-104">**Enrollment profiles**: Preconfigure your devices by platform, enable user affinity, use multi-factor authentication, and more.</span></span>

  <span data-ttu-id="ce986-105">[Mi az eszközök tanúsítványigénylése](https://docs.microsoft.com/intune/device-enrollment), és az [Android](https://docs.microsoft.com/intune/android-enroll), [iOS](https://docs.microsoft.com/intune/ios-enroll), [MacOS](https://docs.microsoft.com/intune/macos-enroll)és [Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) rendszerhez készült igénylési profilok létrehozása jó erőforrás.</span><span class="sxs-lookup"><span data-stu-id="ce986-105">[What is device enrollment](https://docs.microsoft.com/intune/device-enrollment), and create enrollment profiles for [Android](https://docs.microsoft.com/intune/android-enroll), [iOS](https://docs.microsoft.com/intune/ios-enroll), [macOS](https://docs.microsoft.com/intune/macos-enroll), and [Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) are good resources.</span></span>

- <span data-ttu-id="ce986-106">**Megfelelőségi**szabályok: határozza meg, hogy az eszközöknek milyen szabályok és beállítások szerint kell követniük a megfelelőt.</span><span class="sxs-lookup"><span data-stu-id="ce986-106">**Compliance policies**: Define the rules and settings that devices must follow to be compliant.</span></span> <span data-ttu-id="ce986-107">A megfelelőségi házirendekkel is nyomon követheti az eszközöket, és értesítheti a felhasználókat a nem megfelelőségről.</span><span class="sxs-lookup"><span data-stu-id="ce986-107">You can also use compliance policies to monitor devices, and notify users of non-compliance.</span></span>

  <span data-ttu-id="ce986-108">Első lépések az [eszköz megfelelőségi házirendjében](https://docs.microsoft.com/intune/device-compliance-get-started).</span><span class="sxs-lookup"><span data-stu-id="ce986-108">Get started with [device compliance policies](https://docs.microsoft.com/intune/device-compliance-get-started).</span></span>
- <span data-ttu-id="ce986-109">**Feltételes hozzáférés házirendjei**: a megadott feltételektől függően segítséget nyújt a szervezeti erőforrásokhoz.</span><span class="sxs-lookup"><span data-stu-id="ce986-109">**Conditional access policies**: Help secure organizational resources, depending on conditions that you enter.</span></span> <span data-ttu-id="ce986-110">A nem megfelelő eszközök esetén például a feltételes hozzáférés használatával korlátozhatja a levelezéshez és a SharePointhoz való hozzáférést.</span><span class="sxs-lookup"><span data-stu-id="ce986-110">For example, for devices that aren't compliant, use conditional access to restrict access to email and SharePoint.</span></span>

  <span data-ttu-id="ce986-111">A [feltételes hozzáférés és](https://docs.microsoft.com/intune/conditional-access) a [feltételes hozzáférés használatának általános módjai](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) – a kezdéshez hasznos források.</span><span class="sxs-lookup"><span data-stu-id="ce986-111">[What is conditional access](https://docs.microsoft.com/intune/conditional-access) and [common ways to use conditional access](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) are good resources to get started.</span></span>

- <span data-ttu-id="ce986-112">**Konfigurációs profilok**: az eszközök szolgáltatásainak és beállításainak kezelése, például a levelezési beállítások, a WiFi-hálózat hozzáadása, a beépített sablonok használata, az iOS és a MacOS eszköz szolgáltatásainak vezérlése stb.</span><span class="sxs-lookup"><span data-stu-id="ce986-112">**Configuration profiles**: Manage features and settings on devices, including email settings, add a WiFi network, use built-in templates, control iOS and macOS device features, and more.</span></span>

  <span data-ttu-id="ce986-113">Első lépések az [eszköz konfigurációs profiljaiban](https://docs.microsoft.com/intune/device-profiles).</span><span class="sxs-lookup"><span data-stu-id="ce986-113">Get started at [device configuration profiles](https://docs.microsoft.com/intune/device-profiles).</span></span>

<span data-ttu-id="ce986-114">Hasznos hivatkozások:</span><span class="sxs-lookup"><span data-stu-id="ce986-114">Helpful links:</span></span>

- [<span data-ttu-id="ce986-115">Általános kérdések, problémák és felbontások az Intune eszköz házirendjeivel és profiljaival</span><span class="sxs-lookup"><span data-stu-id="ce986-115">Common questions, issues, and resolutions with device policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/device-profile-troubleshoot)

- [<span data-ttu-id="ce986-116">Házirendek és profilok hibaelhárítása az Intune-ban</span><span class="sxs-lookup"><span data-stu-id="ce986-116">Troubleshoot policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
