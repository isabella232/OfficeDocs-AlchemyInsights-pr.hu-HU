---
title: Az örökölt párbeszédpanelek beágyazásának engedélyezése jelentések megnyitásához
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814266"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="8ef0f-102">Az örökölt párbeszédpanelek beágyazásának engedélyezése jelentések megnyitásához</span><span class="sxs-lookup"><span data-stu-id="8ef0f-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="8ef0f-103">**Jelenség**</span><span class="sxs-lookup"><span data-stu-id="8ef0f-103">**Symptom**</span></span>

<span data-ttu-id="8ef0f-104">A felhasználók nem tudnak jelentéseket megnyitni.</span><span class="sxs-lookup"><span data-stu-id="8ef0f-104">Users are unable to open reports.</span></span> <span data-ttu-id="8ef0f-105">„Valami hiba történt.</span><span class="sxs-lookup"><span data-stu-id="8ef0f-105">"Something has gone wrong.</span></span> <span data-ttu-id="8ef0f-106">További részletekért tekintse meg a technikai adatokat.”</span><span class="sxs-lookup"><span data-stu-id="8ef0f-106">Check technical details for more details."</span></span>

<span data-ttu-id="8ef0f-107">**Ok**</span><span class="sxs-lookup"><span data-stu-id="8ef0f-107">**Cause**</span></span>

<span data-ttu-id="8ef0f-108">A jelentések betöltése sikertelen az UCI-ben „Az űrlapleíró null érték vagy nincs megadva“ hibaüzenettel.</span><span class="sxs-lookup"><span data-stu-id="8ef0f-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="8ef0f-109">Az UCI-beli jelentésekhez továbbra is szükségesek az örökölt párbeszédpanelek, így az ügyfélrendszernek engedélyeznie kell az *allowlegacydialogsembedding* beállítást.</span><span class="sxs-lookup"><span data-stu-id="8ef0f-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="8ef0f-110">**Megoldás**</span><span class="sxs-lookup"><span data-stu-id="8ef0f-110">**Solution**</span></span>

1. <span data-ttu-id="8ef0f-111">Válassza a **Beállítások >Felügyelet > Rendszerbeállítások > Általános lap** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="8ef0f-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="8ef0f-112">Állítsa az "Egyes örökölt párbeszédpanelek beágyazásának engedélyezése az Egyesített felület böngészőprogramban" beállítást **Igen** értékre.</span><span class="sxs-lookup"><span data-stu-id="8ef0f-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
