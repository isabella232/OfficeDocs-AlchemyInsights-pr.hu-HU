---
title: EndPoint Manager – Biztonsági alapértékek
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
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/29/2021
ms.locfileid: "51420881"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="0c0a4-102">EndPoint Manager – Biztonsági alapértékek</span><span class="sxs-lookup"><span data-stu-id="0c0a4-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="0c0a4-103">A biztonsági alapértékek a Windows beállításainak előre konfigurált csoportjai, amelyek segítenek a megfelelő biztonsági csoportok által ajánlott biztonsági beállítások alkalmazásában.</span><span class="sxs-lookup"><span data-stu-id="0c0a4-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="0c0a4-104">Ezek az alapértékek testre szabhatók úgy, hogy csak a kívánt beállításokat és értékeket adjanak eredményre.</span><span class="sxs-lookup"><span data-stu-id="0c0a4-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="0c0a4-105">A biztonsági alapértékekkel kapcsolatos további információkért lásd: Windows 10-es eszközök konfigurálása biztonsági alaptervekkel [az Intune-ban.](https://docs.microsoft.com/mem/intune/protect/security-baselines)</span><span class="sxs-lookup"><span data-stu-id="0c0a4-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="0c0a4-106">Ezekhez a termékekhez jelenleg alapértékek vannak:</span><span class="sxs-lookup"><span data-stu-id="0c0a4-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="0c0a4-107">A Windows MDM biztonsági beállításai</span><span class="sxs-lookup"><span data-stu-id="0c0a4-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="0c0a4-108">Microsoft Defender az EndPoint biztonságért</span><span class="sxs-lookup"><span data-stu-id="0c0a4-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="0c0a4-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="0c0a4-109">Microsoft Edge</span></span>

<span data-ttu-id="0c0a4-110">Az alaptervek egyesét rendszeres időközönként frissítjük, és növekményes verziókban adva ki.</span><span class="sxs-lookup"><span data-stu-id="0c0a4-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="0c0a4-111">Minden egyes verzió hozzáadja és eltávolítja az előző verzió beállításait, hogy az alapterv megfeleljen az aktuális útmutatásnak.</span><span class="sxs-lookup"><span data-stu-id="0c0a4-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="0c0a4-112">Az Endpoint Security Security Alaptervek konzolja lehetővé teszi a különböző verziók összehasonlítását úgy, hogy láthatóvá teszi a verzióról verzióra vonatkozó módosításokat.</span><span class="sxs-lookup"><span data-stu-id="0c0a4-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="0c0a4-113">Ha segítségre van szüksége ahhoz, hogy a leghatékonyabban módosítsa az alapterv verzióját, tekintse meg az Alapterv biztonsági profilok kezelése a [Microsoft Intune-ban](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="0c0a4-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="0c0a4-114">Egy biztonsági alapterv telepítése után eszközönként figyelheti a központi telepítés állapotát, és áttekintheti a beállításokat.</span><span class="sxs-lookup"><span data-stu-id="0c0a4-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="0c0a4-115">**Megjegyzés:** Az alaptervek jelentéskészítési adatai akár 24 órát is igénybe vehetnek a kezdeti telepítéstől az eszközig, illetve akár 6 órát is igénybe vehetnek a további frissítések.</span><span class="sxs-lookup"><span data-stu-id="0c0a4-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="0c0a4-116">Az alapterv-beállítások alkalmazásának leggyakoribb oka az, hogy ugyanazt a beállítást használják egy másik profilban.</span><span class="sxs-lookup"><span data-stu-id="0c0a4-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="0c0a4-117">Az adott eszközre vonatkozó eset megvizsgálása az Alap biztonsági alapterv profil Eszköz állapota csomópontján lehetséges.</span><span class="sxs-lookup"><span data-stu-id="0c0a4-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="0c0a4-118">Részletes információkért lásd: [Ütközések feloldása biztonsági alaptervek esetén.](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)</span><span class="sxs-lookup"><span data-stu-id="0c0a4-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>