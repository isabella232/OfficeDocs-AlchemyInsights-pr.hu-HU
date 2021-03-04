---
title: Az Apple automatikus eszközregisztrációs szinkronizálási hibái
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448924"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="0095f-102">Az Apple automatikus eszközregisztrációs szinkronizálási hibái</span><span class="sxs-lookup"><span data-stu-id="0095f-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="0095f-103">"Azt észleltük, hogy egy vagy több ADE/DEP-tokenje van, amelyek hibaállapotban vannak.</span><span class="sxs-lookup"><span data-stu-id="0095f-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="0095f-104">Amíg meg nem oldódik az egyes érintett jogkivonatok hibaállapota, az ADE-funkció nem a várt módon fog működni."</span><span class="sxs-lookup"><span data-stu-id="0095f-104">Until the error state is resolved for each affected token, the ADE functionality will not work as expected.”.</span></span>

<span data-ttu-id="0095f-105">Ez a hiba többféleképpen jelenhet meg:</span><span class="sxs-lookup"><span data-stu-id="0095f-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="0095f-106">Előfordulhat, hogy az eszközök nem szinkronizálódnak az ABM/ASM eszközről az Intune-ba</span><span class="sxs-lookup"><span data-stu-id="0095f-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="0095f-107">Előfordulhat, hogy sikertelenek a regisztrációs profil hozzárendelései</span><span class="sxs-lookup"><span data-stu-id="0095f-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="0095f-108">Előfordulhat, hogy az eszközök nem fejeződnek be sikeresen az ADE-regisztrációval</span><span class="sxs-lookup"><span data-stu-id="0095f-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="0095f-109">Ellenőrizze, hogy nincs-e az Intune konzolon jelentett szinkronizálási hiba az Eszközök > eszköz regisztrálása > Az Apple regisztrációs > **regisztrációs program jogkivonatai között.**</span><span class="sxs-lookup"><span data-stu-id="0095f-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens**.</span></span>

<span data-ttu-id="0095f-110">A szinkronizálási hiba egyik leggyakoribb oka az aktuális jogkivonat lejárata.</span><span class="sxs-lookup"><span data-stu-id="0095f-110">One of the most common causes of sync error is expiration of the current token.</span></span> <span data-ttu-id="0095f-111">Az érintett jogkivonat megújítása sok esetben megoldja a problémát.</span><span class="sxs-lookup"><span data-stu-id="0095f-111">In many cases,renewal of the affected token will resolve the issue.</span></span>

<span data-ttu-id="0095f-112">Ha egy vagy több tokenje lejárt, az alábbi dokumentációban segítséget talál a tokenek szükség szerint való megújításának segítése érdekében:</span><span class="sxs-lookup"><span data-stu-id="0095f-112">If one or more of your tokens has expired,  see the following documentation to help you renew them as appropriate:</span></span>

[<span data-ttu-id="0095f-113">Automatikus eszközregisztrációs jogkivonat megújítása</span><span class="sxs-lookup"><span data-stu-id="0095f-113">Renew an Automated Device Enrollment token</span></span>](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

<span data-ttu-id="0095f-114">Ezenkívül az alábbi dokumentációban láthatja a jogkivonat-szinkronizálási hibákat okozó egyéb hibák esetleges szervizelését:</span><span class="sxs-lookup"><span data-stu-id="0095f-114">In addition, you can see the following documentation to see potential remediations for other errors causing token synchronization failures:</span></span>

[<span data-ttu-id="0095f-115">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span><span class="sxs-lookup"><span data-stu-id="0095f-115">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[<span data-ttu-id="0095f-116">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span><span class="sxs-lookup"><span data-stu-id="0095f-116">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
