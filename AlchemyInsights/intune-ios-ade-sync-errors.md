---
title: Az Apple automatikus eszköz-beiktatási szinkronizálási hibái
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714833"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="f5297-102">Az Apple automatikus eszköz-beiktatási szinkronizálási hibái</span><span class="sxs-lookup"><span data-stu-id="f5297-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="f5297-103">"Észlelték, hogy egy vagy több ADE/DEP-token van, ami egy hibás állapotú.</span><span class="sxs-lookup"><span data-stu-id="f5297-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="f5297-104">Mindaddig, amíg a hiba állapotát meg nem oldotta az egyes érintett jogkivonatok esetében, az ADE-funkció nem fog működni.</span><span class="sxs-lookup"><span data-stu-id="f5297-104">Until the error state is resolved for each affected token, the ADE functionality will not work for the same”.</span></span>

<span data-ttu-id="f5297-105">Ez a hiba többféle módon nyilvánulhat meg, többek között az alábbiakat:</span><span class="sxs-lookup"><span data-stu-id="f5297-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="f5297-106">Lehet, hogy az eszközök nem szinkronizálhatók az ABM/ASM rendszerből a Intune-ra</span><span class="sxs-lookup"><span data-stu-id="f5297-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="f5297-107">Lehet, hogy sikertelenek a tanúsítványigénylési profil hozzárendelései</span><span class="sxs-lookup"><span data-stu-id="f5297-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="f5297-108">Az eszközök nem feltétlenül fejezik be az ADE-regisztrációt</span><span class="sxs-lookup"><span data-stu-id="f5297-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="f5297-109">Ellenőrizze, hogy milyen szinkronizálási hibáról van-e lehetőség a Intune-konzolban az **eszközök > > az Apple tanúsítványigénylési > a beiratkozási program-tokenek** csoportban, és tekintse át az alábbi dokumentumokat a potenciális kármentesítés megtekintéséhez:</span><span class="sxs-lookup"><span data-stu-id="f5297-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens** and review the following documentation to see any potential remediation:</span></span>

[<span data-ttu-id="f5297-110">ABM/ASM szinkronizálási hibák az iOS/iPadOS és a macOS automatikus eszköz-igénylési tokenek esetén</span><span class="sxs-lookup"><span data-stu-id="f5297-110">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
