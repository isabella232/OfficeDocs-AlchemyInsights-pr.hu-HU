---
title: Intune-házirendek és -profilok létrehozása
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1064"
- "6700005"
ms.openlocfilehash: fac2a9e41449b4eb9b87d21d4cba4f6f5192d9c6
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715398"
---
# <a name="creating-intune-policy-and-profiles"></a><span data-ttu-id="fe62d-102">Intune-házirend és -profilok létrehozása</span><span class="sxs-lookup"><span data-stu-id="fe62d-102">Creating Intune policy and profiles</span></span>

<span data-ttu-id="fe62d-103">Az Intune-ban különböző dolgokat használó szabályzatokat és profilokat hozhat létre.</span><span class="sxs-lookup"><span data-stu-id="fe62d-103">In Intune, you can create policies and profiles that do different things.</span></span>

- <span data-ttu-id="fe62d-104">**Regisztrációs profilok:** Az eszközök platformonként történő előzetes konfigurálása, a felhasználói affinitás engedélyezése, a többtényezős hitelesítés használata stb.</span><span class="sxs-lookup"><span data-stu-id="fe62d-104">**Enrollment profiles**: Preconfigure your devices by platform, enable user affinity, use multi-factor authentication, and more.</span></span>

  <span data-ttu-id="fe62d-105">[Mi az eszköz regisztráció](https://docs.microsoft.com/intune/device-enrollment), és hozzon létre regisztrációs profilok [Android,](https://docs.microsoft.com/intune/android-enroll) [iOS](https://docs.microsoft.com/intune/ios-enroll), [macOS](https://docs.microsoft.com/intune/macos-enroll), és a [Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) jó erőforrásokat.</span><span class="sxs-lookup"><span data-stu-id="fe62d-105">[What is device enrollment](https://docs.microsoft.com/intune/device-enrollment), and create enrollment profiles for [Android](https://docs.microsoft.com/intune/android-enroll), [iOS](https://docs.microsoft.com/intune/ios-enroll), [macOS](https://docs.microsoft.com/intune/macos-enroll), and [Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) are good resources.</span></span>

- <span data-ttu-id="fe62d-106">**Megfelelőségi szabályzatok**: Adja meg azokat a szabályokat és beállításokat, amelyeket az eszközöknek követniük kell a megfelelőségérdekében.</span><span class="sxs-lookup"><span data-stu-id="fe62d-106">**Compliance policies**: Define the rules and settings that devices must follow to be compliant.</span></span> <span data-ttu-id="fe62d-107">Megfelelőségi szabályzatok használatával is figyelheti az eszközöket, és értesítheti a felhasználókat a meg nem felelésről.</span><span class="sxs-lookup"><span data-stu-id="fe62d-107">You can also use compliance policies to monitor devices, and notify users of non-compliance.</span></span>

  <span data-ttu-id="fe62d-108">Ismerkedjen meg az [eszközmegfelelőségi szabályzatokkal.](https://docs.microsoft.com/intune/device-compliance-get-started)</span><span class="sxs-lookup"><span data-stu-id="fe62d-108">Get started with [device compliance policies](https://docs.microsoft.com/intune/device-compliance-get-started).</span></span>
- <span data-ttu-id="fe62d-109">**Feltételes hozzáférési házirendek:** A szervezeti erőforrások biztonságossá tétele a megadott feltételektől függően.</span><span class="sxs-lookup"><span data-stu-id="fe62d-109">**Conditional access policies**: Help secure organizational resources, depending on conditions that you enter.</span></span> <span data-ttu-id="fe62d-110">A nem megfelelő eszközök esetében például feltételes hozzáféréssel korlátozhatja az e-mailekhez és a SharePointhoz való hozzáférést.</span><span class="sxs-lookup"><span data-stu-id="fe62d-110">For example, for devices that aren't compliant, use conditional access to restrict access to email and SharePoint.</span></span>

  <span data-ttu-id="fe62d-111">[Mi a feltételes hozzáférés](https://docs.microsoft.com/intune/conditional-access) és [a feltételes hozzáférés használatának gyakori módjai](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) jó erőforrások az első lépésekhez.</span><span class="sxs-lookup"><span data-stu-id="fe62d-111">[What is conditional access](https://docs.microsoft.com/intune/conditional-access) and [common ways to use conditional access](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) are good resources to get started.</span></span>

- <span data-ttu-id="fe62d-112">**Konfigurációs profilok:** Kezelheti az eszközök funkcióit és beállításait, beleértve az e-mail beállításokat, wi-fi hálózatot adhat hozzá, beépített sablonokat használhat, vezérelheti az iOS- és macOS-eszközfunkciókat stb.</span><span class="sxs-lookup"><span data-stu-id="fe62d-112">**Configuration profiles**: Manage features and settings on devices, including email settings, add a WiFi network, use built-in templates, control iOS and macOS device features, and more.</span></span>

  <span data-ttu-id="fe62d-113">Első lépések az [eszközkonfigurációs profilokban.](https://docs.microsoft.com/intune/device-profiles)</span><span class="sxs-lookup"><span data-stu-id="fe62d-113">Get started at [device configuration profiles](https://docs.microsoft.com/intune/device-profiles).</span></span>

<span data-ttu-id="fe62d-114">Hasznos linkek:</span><span class="sxs-lookup"><span data-stu-id="fe62d-114">Helpful links:</span></span>

- [<span data-ttu-id="fe62d-115">Gyakori kérdések, problémák és megoldások az Intune-ban lévő eszközházirendekkel és -profilokkal</span><span class="sxs-lookup"><span data-stu-id="fe62d-115">Common questions, issues, and resolutions with device policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/device-profile-troubleshoot)

- [<span data-ttu-id="fe62d-116">Házirendek és profilok – problémamegoldás az Intune-ban</span><span class="sxs-lookup"><span data-stu-id="fe62d-116">Troubleshoot policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
