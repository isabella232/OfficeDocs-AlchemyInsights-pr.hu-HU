---
title: A Nem sikerült észlelni az alkalmazást hiba előfordulásainak csökkentése
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: e07c6b128a39f1fb1c998d051aafe72205d8cbee
ms.sourcegitcommit: 82155846ce771c18050e6113d6c199b34a1504ff
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/24/2020
ms.locfileid: "43810486"
---
# <a name="mitigate-the-application-was-not-detected-error"></a><span data-ttu-id="40fb8-102">A „Nem sikerült észlelni az alkalmazást” hiba előfordulásainak csökkentése</span><span class="sxs-lookup"><span data-stu-id="40fb8-102">Mitigate "The application was not detected" error</span></span>

<span data-ttu-id="40fb8-103">Az Intune által jelentett „Nem sikerült észlelni az alkalmazást a telepítés sikeres befejezése után” alkalmazástelepítési hiba az összes fontos operációs rendszeren (Windows, iOS és Android) jelentkezhet.</span><span class="sxs-lookup"><span data-stu-id="40fb8-103">The app installation error, “The application was not detected after installation completed successfully,” reported by Intune, may occur on all major OS platforms (Windows, iOS and Android).</span></span>

<span data-ttu-id="40fb8-104">A hibát kiváltó leggyakoribb esetek közé tartoznak a következők:</span><span class="sxs-lookup"><span data-stu-id="40fb8-104">The most common scenarios that generate this error include:</span></span>

- <span data-ttu-id="40fb8-105">A kezdeti rendszerbe állítást követően az Intune-on kívül frissítették az alkalmazást (harmadik fél alkalmazás-áruházából).</span><span class="sxs-lookup"><span data-stu-id="40fb8-105">The app has been updated outside of Intune (from a third-party app store) after the initial deployment.</span></span> <span data-ttu-id="40fb8-106">Előfordulhat például, hogy bizonyos alkalmazások – mint például a Google Chrome – automatikus frissítéseket hajtanak végre.</span><span class="sxs-lookup"><span data-stu-id="40fb8-106">For example some applications such as Google Chrome may perform auto updates.</span></span>
- <span data-ttu-id="40fb8-107">Egy felhasználó eltávolította az alkalmazást annak kezdeti telepítése után.</span><span class="sxs-lookup"><span data-stu-id="40fb8-107">A user has uninstalled the app after the initial install.</span></span>

<span data-ttu-id="40fb8-108">A probléma megoldásához először ellenőrizze az érintett eszközöket, hogy megállapíthassa, melyik eset vezet a hibához.</span><span class="sxs-lookup"><span data-stu-id="40fb8-108">To mitigate this issue, first perform a review of the affected devices to determine the scenario in which the error occurs.</span></span>

- <span data-ttu-id="40fb8-109">Ha az Intune-on kívül frissítették az alkalmazást, akkor az alkalmazás üzemeltetése beállítható úgy, hogy figyelmen kívül hagyja az alkalmazás verziószámát.</span><span class="sxs-lookup"><span data-stu-id="40fb8-109">If the app has been updated outside of Intune, the app deployment can be set to ignore the application version.</span></span> <span data-ttu-id="40fb8-110">Ehhez állítsa **Igen** értékre az **Alkalmazás konfigurációja > Alkalmazásadatok** csoportban levő **Alkalmazás verziójának figyelmen kívül hagyása** beállítást.</span><span class="sxs-lookup"><span data-stu-id="40fb8-110">To do so, under **App Configuration > App Information**, set **Ignore App** version to **Yes**.</span></span>
- <span data-ttu-id="40fb8-111">Az ügyfél célzásakor célszerű lehet „kötelező” módon telepíteni az alkalmazást, és biztosítani, hogy a legújabb verzió legyen rendszerbe állítva.</span><span class="sxs-lookup"><span data-stu-id="40fb8-111">When targeting the client, it may be appropriate to deploy the application as “required,” and to ensure that the latest version is deployed.</span></span>
- <span data-ttu-id="40fb8-112">Az iOS platformon azt is megteheti, hogy az Apple mennyiségi vásárlási programjához társított **automatikus frissítési** funkciót használja, amely konfigurálható úgy, hogy automatikusan frissítsen az új alkalmazásverziókra, amint azok elérhetővé válnak.</span><span class="sxs-lookup"><span data-stu-id="40fb8-112">Alternatively, on the iOS platform, it is possible to use the **autoupdate** functionality associated with the Apple Volume Purchase Program, which can be configured to automatically update to new application versions as they become available.</span></span>

<span data-ttu-id="40fb8-113">Az alkalmazások telepítésével kapcsolatos hibák elhárításáról az [Alkalmazástelepítési problémák elhárítása](https://docs.microsoft.com/intune/troubleshoot-app-install) című témakörben olvashat bővebben.</span><span class="sxs-lookup"><span data-stu-id="40fb8-113">For more information about troubleshooting app installation issues, please see [Troubleshoot app installation issues](https://docs.microsoft.com/intune/troubleshoot-app-install).</span></span>
