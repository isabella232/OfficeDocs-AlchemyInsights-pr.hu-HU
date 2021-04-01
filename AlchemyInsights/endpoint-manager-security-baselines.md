---
title: Endpoint Manager – Biztonsági alaptervek
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440886"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="506f9-102">Endpoint Manager – Biztonsági alaptervek</span><span class="sxs-lookup"><span data-stu-id="506f9-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="506f9-103">A biztonsági alaptervek előre konfigurált Windows beállítások csoportja, amelyek segítenek Önnek alkalmazni azokat a beállításokat, amelyet a releváns biztonsági csoportok ajánlottak.</span><span class="sxs-lookup"><span data-stu-id="506f9-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="506f9-104">Ezeket az alapterveket testre lehet szabni, hogy csak a kívánt beállításokat és értékeket adják vissza.</span><span class="sxs-lookup"><span data-stu-id="506f9-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="506f9-105">További információkért a biztonsági alaptervekről, lásd a [Biztonsági alaptervek használata a Windows 10 eszközök Intune-ban való konfigurálásához](https://docs.microsoft.com/mem/intune/protect/security-baselines)menüpontot.</span><span class="sxs-lookup"><span data-stu-id="506f9-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="506f9-106">Jelenleg ezekhez a termékekhez találhatók alaptervek:</span><span class="sxs-lookup"><span data-stu-id="506f9-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="506f9-107">Windows MDM Biztonsági beállítások</span><span class="sxs-lookup"><span data-stu-id="506f9-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="506f9-108">Végponthoz készült Microsoft Defender Biztonság</span><span class="sxs-lookup"><span data-stu-id="506f9-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="506f9-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="506f9-109">Microsoft Edge</span></span>

<span data-ttu-id="506f9-110">Mindegyik alaptervet időszakosan frissítjük és lépésenkénti verziókban adjuk ki.</span><span class="sxs-lookup"><span data-stu-id="506f9-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="506f9-111">Mindegyik verzió hozzáad, vagy eltávolít beállításokat az előző verziókból annak érdekében, hogy az alapterv az aktuális útmutatásnak megfelelő legyen.</span><span class="sxs-lookup"><span data-stu-id="506f9-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="506f9-112">A Biztonsági alapterv konzolja a Végpont biztonságban lehetővé teszi a különböző verziók összehasonlítását azáltal, hogy láthatóvá teszi a verziónkénti változtatásokat.</span><span class="sxs-lookup"><span data-stu-id="506f9-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="506f9-113">Ahhoz az útmutatáshoz, hogy leghatékonyabban lehessen módosítani, melyik alapterv van üzembe helyezve, lásd a [Biztonsági alapterv-profilok kezelése a Microsoft Intune-ban](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure) lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="506f9-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="506f9-114">A biztonsági alapterv üzemebe helyezése után megfigyelheti az üzembe helyezés állapotát és áttekintheti a beállításokat eszközről eszközre.</span><span class="sxs-lookup"><span data-stu-id="506f9-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="506f9-115">**Megjegyzés:** Az alaptervek jelentési adatának megjelenése akár 24 órát is igénybe vehet az eszközre való telepítés előkészítésétől, és akár 6 órát is a további frissítéseknél.</span><span class="sxs-lookup"><span data-stu-id="506f9-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="506f9-116">A leggyakoribb oka annak, ha egy alapterv-beállítás nem alkalmazható az, hogy ugyanazt a beállítást már egy másik profilban is használják.</span><span class="sxs-lookup"><span data-stu-id="506f9-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="506f9-117">Bizonyos eszköznél ki lehet vizsgálni ezt a forgatókönyvet a Biztonsági alapterv profiljának Eszközállapot csomópontjából.</span><span class="sxs-lookup"><span data-stu-id="506f9-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="506f9-118">További részletekért lásd a [Biztonsági alaptervek konfliktusainak megoldása](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines) menüpontot.</span><span class="sxs-lookup"><span data-stu-id="506f9-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>