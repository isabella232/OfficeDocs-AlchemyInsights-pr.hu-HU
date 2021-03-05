---
title: Probléma az attribútum- és hatókör-szűrési szűrővel
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481892"
---
# <a name="problem-with-attribute-and-scoping-filter"></a><span data-ttu-id="70629-102">Probléma az attribútum- és hatókör-szűrési szűrővel</span><span class="sxs-lookup"><span data-stu-id="70629-102">Problem with attribute and scoping filter</span></span>

<span data-ttu-id="70629-103">**Probléma az ütköző UPN-értékekkel**</span><span class="sxs-lookup"><span data-stu-id="70629-103">**Issue with conflicting UPN values**</span></span>

<span data-ttu-id="70629-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique.**</span><span class="sxs-lookup"><span data-stu-id="70629-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span></span> <span data-ttu-id="70629-105">A művelet nem sikerült, mert az összeadáshoz/módosításhoz megadott UPN-érték nem egyedi erdőszintű.</span><span class="sxs-lookup"><span data-stu-id="70629-105">The operation failed because UPN value provided for addition/modification is not unique forest-wide.</span></span> <span data-ttu-id="70629-106">Hiba részletei: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="70629-106">Error Details: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span></span>

<span data-ttu-id="70629-107">Az **a userPrincipalName érték,** amit a Workday-összekötő próbál beállítani az AD felhasználói fiók létrehozásakor, már létezik a cél AD tartományban.</span><span class="sxs-lookup"><span data-stu-id="70629-107">The **userPrincipalName** value that Workday connector is trying to set when creating the AD user account already exists in the target AD domain.</span></span> <span data-ttu-id="70629-108">Ez azt jelenti, hogy vagy (1) már létezik a felhasználó, és az egyező azonosító ellenőrzése sikertelen volt a felhasználónál, vagy (2) az UPN-generációs szabály ütköző értéket generált.</span><span class="sxs-lookup"><span data-stu-id="70629-108">This implies that either (1) the user already exists and the matching ID check failed for the user or (2) the UPN generation rule generated a conflicting value.</span></span>

<span data-ttu-id="70629-109">Íme a javasolt megoldási lépések:</span><span class="sxs-lookup"><span data-stu-id="70629-109">Here are the suggested resolution steps:</span></span>

<span data-ttu-id="70629-110">Ha a felhasználó már létezik, és a megfelelő azonosító-ellenőrzés nem tudta összekapcsolni a Workday-fiókot az Active Directory-fiókkal, akkor ellenőrizze, hogy a Workday és az AD azonosítójának egyező attribútuma (jellemzően **employeeID)** pontosan egyezik-e.</span><span class="sxs-lookup"><span data-stu-id="70629-110">If the user already exists and the matching ID check failed to link the Workday account to Active Directory account, then check if the matching ID attribute (typically **employeeID**) in both Workday and AD have an exact match.</span></span> <span data-ttu-id="70629-111">Ha nincs egyezésük, azt az adat problémáját kell kijavítanunk.</span><span class="sxs-lookup"><span data-stu-id="70629-111">If they don't have a match, it is a data issue that needs to be fixed.</span></span> <span data-ttu-id="70629-112">Ha például a Workday alkalmazottazonosítója 001052, az AD-ben pedig 1052, akkor a kiépítési motor nem tudja összekapcsolni a két fiókot, és megpróbál létrehozni egy már létező felhasználót.</span><span class="sxs-lookup"><span data-stu-id="70629-112">For example, if the EmployeeID in Workday is 001052 and in AD it is 1052, then the provisioning engine will fail to link the two accounts and will try to create a user that already exists.</span></span> <span data-ttu-id="70629-113">Ebben az esetben úgy kell  módosítania az Alkalmazottazonosító értékét az AD-ben, hogy az tartalmazza a kezdő nullákat, hogy 001052 legyen.</span><span class="sxs-lookup"><span data-stu-id="70629-113">The solution in this case is to change the **EmployeeID** value in AD to include the leading zeros to make it 001052.</span></span>
<span data-ttu-id="70629-114">Ha az UPN-et generáló kifejezés nem hoz létre egyedi értéket, érdemes lehet a **SelectUniqueValue** duplikálásának függvényével minden alkalommal egyedi értéket létrehozni.</span><span class="sxs-lookup"><span data-stu-id="70629-114">If the UPN-generating expression is not generating a unique value, consider using the de-duplication function **SelectUniqueValue** to generate a unique value each time.</span></span>

<span data-ttu-id="70629-115">**Az AD-felhasználó kiépítésének munkanapja nem ad meg kezelői attribútumértéket az AD-felhasználói fiókhoz**</span><span class="sxs-lookup"><span data-stu-id="70629-115">**Workday to AD User Provisioning does not set manager attribute value for AD user account**</span></span>

<span data-ttu-id="70629-116">Az AD-felhasználó kiépítési feladata nem  a kezelő attribútumértékének beállítása az AD-felhasználói fiókokhoz.</span><span class="sxs-lookup"><span data-stu-id="70629-116">The Workday to AD User Provisioning job is not setting the **manager** attribute value for AD user accounts.</span></span> <span data-ttu-id="70629-117">Ennek a viselkedésnek két lehetséges forgatókönyve van:</span><span class="sxs-lookup"><span data-stu-id="70629-117">There are two possible scenarios when this behavior is seen:</span></span>

1. <span data-ttu-id="70629-118">A Workdayben a vezető nem oldható fel egy megfelelő AD-felhasználói fiókkal, mert a vezető nincs hatókörben.</span><span class="sxs-lookup"><span data-stu-id="70629-118">The manager in Workday cannot be resolved to a corresponding AD User account because the manager is not in scope.</span></span>
2. <span data-ttu-id="70629-119">Több **AD-tartomány** esetén a Workday kezelője nem ugyanabban a tartományban van, mint a felhasználó.</span><span class="sxs-lookup"><span data-stu-id="70629-119">In a **multiple AD domains** scenario, the manager in Workday is not present in the same domain as the user.</span></span>

<span data-ttu-id="70629-120">A probléma megoldásához próbálkozzon az alábbi lépésekkel:</span><span class="sxs-lookup"><span data-stu-id="70629-120">Try these steps to resolve the issue:</span></span>

1. <span data-ttu-id="70629-121">Ha hatókör-meghatározási szűrőket definiált, először ellenőrizze, hogy a kezelő hatóköre kiterjed-e, és hogy megfelel-e a hatókör-meghatározási záradéknak.</span><span class="sxs-lookup"><span data-stu-id="70629-121">If you have defined scoping filters, first check if the manager is in scope and that it satisfies the scoping clause.</span></span> <span data-ttu-id="70629-122">Ha a vezető nem felel meg a hatókör-szűrési szűrőnek, módosítsa úgy a szűrőt, hogy a kezelő a kiépítési művelet hatókörében is kiterjedni.</span><span class="sxs-lookup"><span data-stu-id="70629-122">If the manager does not satisfy the scoping filter, change the filter so that the manager is also in scope of the provisioning operation.</span></span>
2. <span data-ttu-id="70629-123">Ha több AD-tartománya van, akkor az összekötőben ismert korlátozás van, hogy nem lehet feloldani a tartományközi kezelői hivatkozásokat.</span><span class="sxs-lookup"><span data-stu-id="70629-123">If you have multiple AD domains, then the connector has a known limitation of inability to resolve cross-domain manager references.</span></span>

<span data-ttu-id="70629-124">A munkanap automatikus kiépítéshez való konfigurálásával kapcsolatos további információkért lásd: A Munkanap beállítása automatikus felhasználói [kiépítéshez.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="70629-124">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>













