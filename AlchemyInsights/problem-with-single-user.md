---
title: Probléma egyetlen felhasználóval
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
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429715"
---
# <a name="problem-with-single-user"></a><span data-ttu-id="d5db3-102">Probléma egyetlen felhasználóval</span><span class="sxs-lookup"><span data-stu-id="d5db3-102">Problem with single user</span></span>

- <span data-ttu-id="d5db3-103">Előfordulhat, hogy a felhasználó nem lett kiépítve, mert a szolgáltatásnak még nem volt lehetősége kiértékelni a felhasználót.</span><span class="sxs-lookup"><span data-stu-id="d5db3-103">The user may not have been provisioned because the service hasn't had a chance to evaluate the user yet.</span></span> <span data-ttu-id="d5db3-104">Tekintse át az útmutatót, hogy mennyi ideig tart a kiépítés, valamint a kiépítési konfigurációs lap folyamatjelző sávja.</span><span class="sxs-lookup"><span data-stu-id="d5db3-104">Review the guidance for how long provisioning takes as well as the progress bar on the provisioning configuration page.</span></span> <span data-ttu-id="d5db3-105">Ha a további részletek szakaszban megadott egyenletes állapot a felhasználó létrehozási/frissítés/törlési dátuma előtt áll, az azt jelenti, hogy még nem értékeltük ki a felhasználót.</span><span class="sxs-lookup"><span data-stu-id="d5db3-105">If the steady state specified in the additional details section is before the date the user was created/updated/deleted, it means we have not evaluated the user yet.</span></span> <span data-ttu-id="d5db3-106">Ebben az esetben a legjobb, ha megvárja, amíg befejeződik a kiépítési szolgáltatás.</span><span class="sxs-lookup"><span data-stu-id="d5db3-106">In this scenario, the best thing to do is wait for the provisioning service to finish.</span></span>

  - <span data-ttu-id="d5db3-107">Felhívjuk a figyelmét arra, hogy szolgáltatásunk csak a forrásrendszerben (felhőbeli HR) felhasználó módosításait ismeri.</span><span class="sxs-lookup"><span data-stu-id="d5db3-107">Note that our service is only aware of changes to a user in the source system (Cloud HR).</span></span> <span data-ttu-id="d5db3-108">Az Azure AD-nek érvényes változásnak kell lennie a forrásrendszerben ahhoz, hogy észlelje a változást, és átfolyta azt az Active Directoryba.</span><span class="sxs-lookup"><span data-stu-id="d5db3-108">There has to be a valid change in the source system for Azure AD to detect the change and flow it into Active Directory.</span></span>
- <span data-ttu-id="d5db3-109">A kiépítési szolgáltatás kiértékelte a felhasználót, és megállapította, hogy nem szükséges kiépítve:</span><span class="sxs-lookup"><span data-stu-id="d5db3-109">Provisioning service evaluated the user and determined it should not be provisioned:</span></span>
  - <span data-ttu-id="d5db3-110">Ha beállított egy attribútumalapú hatókör-szűrési szűrőt, győződjön meg arról, hogy a felhasználó megfelel az Ön által megadott feltételeknek.</span><span class="sxs-lookup"><span data-stu-id="d5db3-110">If you have set an attribute based scoping filter, ensure that the user meets the criteria that you have specified.</span></span>
  - <span data-ttu-id="d5db3-111">Ha a felhasználók már léteznek a célrendszerben, és a felhasználó állapota a forrás- és cél egyezésben, nem tudunk semmilyen további műveletet.</span><span class="sxs-lookup"><span data-stu-id="d5db3-111">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span></span>
- <span data-ttu-id="d5db3-112">A kiépítési szolgáltatás megkísérelte kiépítni a felhasználót, és az nem sikerült.</span><span class="sxs-lookup"><span data-stu-id="d5db3-112">Provisioning service attempted to provision the user and it failed.</span></span> <span data-ttu-id="d5db3-113">Ilyen esetekben tekintse át a kiépítési naplók hibaelhárítási és javaslatok lapját:</span><span class="sxs-lookup"><span data-stu-id="d5db3-113">For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:</span></span>
  - <span data-ttu-id="d5db3-114">Előfordulhat, hogy a felhasználó egy kötelező attribútuma hiányzik a helyszíni Active Directoryból vagy az Azure AD-ből.</span><span class="sxs-lookup"><span data-stu-id="d5db3-114">A required attribute on the user might be missing in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="d5db3-115">A userPrincipalName vagy sAMAccountName generációs szabályok például nem a megfelelő értéket generálják.</span><span class="sxs-lookup"><span data-stu-id="d5db3-115">For example, the userPrincipalName or sAMAccountName generation rules are not generating the right value.</span></span>
  - <span data-ttu-id="d5db3-116">Az egyező attribútum (általában employeeId) nem megoldás egy egyedi felhasználónál a helyszíni Active Directoryban vagy az Azure AD-ban.</span><span class="sxs-lookup"><span data-stu-id="d5db3-116">The matching attribute (usually employeeId) is not resolving to a unique user in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="d5db3-117">Két felhasználónak például ugyanaz az alkalmazottazonosítója van az AD-ban, és a szolgáltatás hibaüzenetet ad vissza, amely ugyanazt a forrásbejegyzést jelzi duplikált célbejegyzésként.</span><span class="sxs-lookup"><span data-stu-id="d5db3-117">For example, there are two users with the same employeeId in AD and the service returns an error code indicate duplicate target entries for the same source entry.</span></span>

<span data-ttu-id="d5db3-118">Az egyes felhasználók és csoportok naplóit a kiépítési naplók áttekintése egy adott felhasználóval kapcsolatos [problémához olvassa el.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)</span><span class="sxs-lookup"><span data-stu-id="d5db3-118">To review logs for single user and groups, see [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span></span>
