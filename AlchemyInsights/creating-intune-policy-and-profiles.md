---
title: Intune házirendek és profilok létrehozása
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 05/07/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 6700005
ms.openlocfilehash: 3fecad7d02b8e3148a3dd774d666fc4ed317204c
ms.sourcegitcommit: 7e2122a7e08525f628986978f396b3a138d2326d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/07/2019
ms.locfileid: "33661737"
---
# <a name="creating-intune-policy-and-profiles"></a><span data-ttu-id="1548b-102">Intune házirend és profilok létrehozása</span><span class="sxs-lookup"><span data-stu-id="1548b-102">Creating Intune policy and profiles</span></span>

<span data-ttu-id="1548b-103">Intune politikák és különböző dologra profilokat hozhat létre.</span><span class="sxs-lookup"><span data-stu-id="1548b-103">In Intune, you can create policies and profiles that do different things.</span></span>

- <span data-ttu-id="1548b-104">**Beiktatási profilok**: az eszközök előzetes platform, felhasználói affinitás engedélyezése, többtényezős hitelesítést és több.</span><span class="sxs-lookup"><span data-stu-id="1548b-104">**Enrollment profiles**: Preconfigure your devices by platform, enable user affinity, use multi-factor authentication, and more.</span></span> 

  <span data-ttu-id="1548b-105">[Mi az eszköz beiktató](https://docs.microsoft.com/intune/device-enrollment), és [Android](https://docs.microsoft.com/intune/android-enroll), [iOS](https://docs.microsoft.com/intune/ios-enroll), [macOS](https://docs.microsoft.com/intune/macos-enroll)tagság profilokat hozhat létre, és [a Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) megfelelő erőforrásokat.</span><span class="sxs-lookup"><span data-stu-id="1548b-105">[What is device enrollment](https://docs.microsoft.com/intune/device-enrollment), and create enrollment profiles for [Android](https://docs.microsoft.com/intune/android-enroll), [iOS](https://docs.microsoft.com/intune/ios-enroll), [macOS](https://docs.microsoft.com/intune/macos-enroll), and [Windows](https://docs.microsoft.com/intune/windows-enrollment-methods) are good resources.</span></span>

- <span data-ttu-id="1548b-106">**Megfelelési politikák**: a szabályok és eszközök kell követnie kell a megfelelő beállítások megadása.</span><span class="sxs-lookup"><span data-stu-id="1548b-106">**Compliance policies**: Define the rules and settings that devices must follow to be compliant.</span></span> <span data-ttu-id="1548b-107">Megfelelési házirendek segítségével figyelheti az eszközök, és értesítheti a felhasználókat a meg nem felelés is.</span><span class="sxs-lookup"><span data-stu-id="1548b-107">You can also use compliance policies to monitor devices, and notify users of non-compliance.</span></span> 

  <span data-ttu-id="1548b-108">[Megfelelés irányelveinek eszköz](https://docs.microsoft.com/intune/device-compliance-get-started)használatának megkezdéséhez.</span><span class="sxs-lookup"><span data-stu-id="1548b-108">Get started with [device compliance policies](https://docs.microsoft.com/intune/device-compliance-get-started).</span></span>
- <span data-ttu-id="1548b-109">**Feltételes hozzáférési házirendek**: Súgó biztonságos vállalati erőforrást a megadott feltételektől függően.</span><span class="sxs-lookup"><span data-stu-id="1548b-109">**Conditional access policies**: Help secure organizational resources, depending on conditions that you enter.</span></span> <span data-ttu-id="1548b-110">Például olyan eszközök, amelyek nem kompatibilis, használja a hozzáférés korlátozása az e-mail és a SharePoint feltételes hozzáférésű.</span><span class="sxs-lookup"><span data-stu-id="1548b-110">For example, for devices that aren't compliant, use conditional access to restrict access to email and SharePoint.</span></span>

  <span data-ttu-id="1548b-111">[Mi a feltételes hozzáférésű](https://docs.microsoft.com/intune/conditional-access) és [leggyakoribb használatával feltételes hozzáférésű](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) jó források a kezdéshez.</span><span class="sxs-lookup"><span data-stu-id="1548b-111">[What is conditional access](https://docs.microsoft.com/intune/conditional-access) and [common ways to use conditional access](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use) are good resources to get started.</span></span>

- <span data-ttu-id="1548b-112">**Konfigurációs profilok**: szolgáltatások és eszközök, beleértve az e-mail beállításait a beállítások kezelése, WiFi hálózathoz hozzáadni, használja a beépített sablonok, ellenőrzés iOS és macOS eszköz szolgáltatásait és több.</span><span class="sxs-lookup"><span data-stu-id="1548b-112">**Configuration profiles**: Manage features and settings on devices, including email settings, add a WiFi network, use built-in templates, control iOS and macOS device features, and more.</span></span> 

  <span data-ttu-id="1548b-113">Ismerkedés a [eszköz konfigurációs profilok](https://docs.microsoft.com/intune/device-profiles).</span><span class="sxs-lookup"><span data-stu-id="1548b-113">Get started at [device configuration profiles](https://docs.microsoft.com/intune/device-profiles).</span></span>

<span data-ttu-id="1548b-114">Hasznos hivatkozásokat:</span><span class="sxs-lookup"><span data-stu-id="1548b-114">Helpful links:</span></span>

- [<span data-ttu-id="1548b-115">Gyakori kérdések, problémák és megoldások eszköz politikákkal és Intune a profilok</span><span class="sxs-lookup"><span data-stu-id="1548b-115">Common questions, issues, and resolutions with device policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/device-profile-troubleshoot)

- [<span data-ttu-id="1548b-116">Házirendek és Intune a profilok – problémamegoldás</span><span class="sxs-lookup"><span data-stu-id="1548b-116">Troubleshoot policies and profiles in Intune</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)