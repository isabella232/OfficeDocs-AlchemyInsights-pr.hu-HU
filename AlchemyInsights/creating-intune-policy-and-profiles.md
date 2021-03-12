---
title: Intune-házirendek és -profilok létrehozása
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
ms.openlocfilehash: af8f1a3dfaccaca52f187f387274d63b22631b2d
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704644"
---
# <a name="creating-intune-policy-and-profiles"></a><span data-ttu-id="9aa2d-102">Intune-házirendek és -profilok létrehozása</span><span class="sxs-lookup"><span data-stu-id="9aa2d-102">Creating Intune policy and profiles</span></span>

<span data-ttu-id="9aa2d-103">Az Intune-ban létrehozhat különböző funkciókat ható házirendeket és profilokat.</span><span class="sxs-lookup"><span data-stu-id="9aa2d-103">In Intune, you can create policies and profiles that do different things.</span></span>

- <span data-ttu-id="9aa2d-104">**Regisztrációs profilok:** Előkonfigurálhatja az eszközeit platform szerint, engedélyezheti a felhasználói érdeklődést, többtényezős hitelesítést használhat stb.</span><span class="sxs-lookup"><span data-stu-id="9aa2d-104">**Enrollment profiles**: Preconfigure your devices by platform, enable user affinity, use multi-factor authentication, and more.</span></span>

  <span data-ttu-id="9aa2d-105">[Az androidos,](https://docs.microsoft.com/intune/device-enrollment) [iOS-,](https://docs.microsoft.com/intune/ios-enroll) [macOS-](https://docs.microsoft.com/intune/macos-enroll)és [Windowsos](https://docs.microsoft.com/intune/windows-enrollment-methods) eszközök regisztrálása és regisztrációs profilok létrehozása. [](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="9aa2d-105">[What is device enrollment](https://docs.microsoft.com/intune/device-enrollment), and create enrollment profiles for [Android](https://docs.microsoft.com/intune/android-enroll), [iOS](https://docs.microsoft.com/intune/ios-enroll), [macOS](https://docs.microsoft.com/intune/macos-enroll), and [Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) are good resources.</span></span>

- <span data-ttu-id="9aa2d-106">**Megfelelőségi szabályzatok:** Határozza meg azokat a szabályokat és beállításokat, amelyek betartásához az eszközöknek meg kell felelnie.</span><span class="sxs-lookup"><span data-stu-id="9aa2d-106">**Compliance policies**: Define the rules and settings that devices must follow to be compliant.</span></span> <span data-ttu-id="9aa2d-107">Megfelelőségi szabályzatok használatával figyelheti az eszközöket, és értesítheti a felhasználókat a nem megfelelőségről.</span><span class="sxs-lookup"><span data-stu-id="9aa2d-107">You can also use compliance policies to monitor devices, and notify users of non-compliance.</span></span>

  <span data-ttu-id="9aa2d-108">Az eszköz-megfelelőségi [szabályzatok használata – első lépések](https://docs.microsoft.com/intune/device-compliance-get-started)</span><span class="sxs-lookup"><span data-stu-id="9aa2d-108">Get started with [device compliance policies](https://docs.microsoft.com/intune/device-compliance-get-started).</span></span>
- <span data-ttu-id="9aa2d-109">**Feltételes hozzáférési házirendek:** A szervezeti erőforrások biztonságának biztosítása a beírott feltételektől függően.</span><span class="sxs-lookup"><span data-stu-id="9aa2d-109">**Conditional access policies**: Help secure organizational resources, depending on conditions that you enter.</span></span> <span data-ttu-id="9aa2d-110">Ha például az eszközök nem kompatibilisek, feltételes hozzáféréssel korlátozhatja a levelezéshez és a SharePointhoz való hozzáférést.</span><span class="sxs-lookup"><span data-stu-id="9aa2d-110">For example, for devices that aren't compliant, use conditional access to restrict access to email and SharePoint.</span></span>

  <span data-ttu-id="9aa2d-111">[A feltételes](https://docs.microsoft.com/intune/conditional-access) hozzáférés [](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) és a feltételes hozzáférés általános módjai jó források az első lépésekhez.</span><span class="sxs-lookup"><span data-stu-id="9aa2d-111">[What is conditional access](https://docs.microsoft.com/intune/conditional-access) and [common ways to use conditional access](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) are good resources to get started.</span></span>

- <span data-ttu-id="9aa2d-112">**Konfigurációs profilok:** Kezelheti az eszközökön található szolgáltatásokat és beállításokat, többek között az e-mail-beállításokat, Wi-Fi hálózatot adhat hozzá, beépített sablonokat használhat, szabályozhatja az iOS és a macOS eszköz funkcióit stb.</span><span class="sxs-lookup"><span data-stu-id="9aa2d-112">**Configuration profiles**: Manage features and settings on devices, including email settings, add a WiFi network, use built-in templates, control iOS and macOS device features, and more.</span></span>

  <span data-ttu-id="9aa2d-113">Első lépések az [eszközkonfigurációs profiloknál.](https://docs.microsoft.com/intune/device-profiles)</span><span class="sxs-lookup"><span data-stu-id="9aa2d-113">Get started at [device configuration profiles](https://docs.microsoft.com/intune/device-profiles).</span></span>

<span data-ttu-id="9aa2d-114">Hasznos hivatkozások:</span><span class="sxs-lookup"><span data-stu-id="9aa2d-114">Helpful links:</span></span>

- [<span data-ttu-id="9aa2d-115">Eszköz házirendekkel és profilokkal kapcsolatos gyakori kérdések, problémák és megoldások az Intune-ban</span><span class="sxs-lookup"><span data-stu-id="9aa2d-115">Common questions, issues, and resolutions with device policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/device-profile-troubleshoot)

- [<span data-ttu-id="9aa2d-116">Házirendek és profilok hibaelhárítása az Intune-ban</span><span class="sxs-lookup"><span data-stu-id="9aa2d-116">Troubleshoot policies and profiles in Intune</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)
