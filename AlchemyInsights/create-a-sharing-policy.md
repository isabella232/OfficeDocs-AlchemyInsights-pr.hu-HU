---
title: Megosztási házirend létrehozása, hogy a felhasználók megosszák naptárukat a szervezeten kívüli emberekkel
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
- "3800014"
- "898"
ms.openlocfilehash: 016b915a9e8f7e32d5d393bc47347991866647c7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816274"
---
# <a name="create-a-sharing-policy-to-allow-your-users-to-share-their-calendar-with-people-outside-your-organization"></a><span data-ttu-id="f553a-102">Megosztási házirend létrehozása, hogy a felhasználók megosszák naptárukat a szervezeten kívüli emberekkel</span><span class="sxs-lookup"><span data-stu-id="f553a-102">Create a Sharing Policy to allow your users to share their calendar with people outside your organization</span></span>

1. <span data-ttu-id="f553a-103">A Microsoft 365 Felügyeleti központ irányítópultján menjen a **Felügyeleti exchange**  >  **lapra.**</span><span class="sxs-lookup"><span data-stu-id="f553a-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="f553a-104">Ugrás a **szervezet**  >  **megosztására .**</span><span class="sxs-lookup"><span data-stu-id="f553a-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="f553a-105">A listanézet Egyéni megosztás **listájában kattintson** az Új **elemre.**</span><span class="sxs-lookup"><span data-stu-id="f553a-105">In the list view, under **Individual Sharing**, click **New** .</span></span>
4. <span data-ttu-id="f553a-106">Az **új megosztási házirendben** írjon be egy rövid nevet a megosztási házirendnek a Házirend **neve mezőbe.**</span><span class="sxs-lookup"><span data-stu-id="f553a-106">In **new sharing policy**, type a friendly name for the sharing policy in the **Policy name** box.</span></span>
5. <span data-ttu-id="f553a-107">Kattintson **a Hozzáadás**  gombra a házirend megosztási szabályainak meghatározásához.</span><span class="sxs-lookup"><span data-stu-id="f553a-107">Click **Add**  to define the sharing rules for the policy.</span></span>
6. <span data-ttu-id="f553a-108">A **megosztási szabályban** az alábbi lehetőségek közül választva adja meg, hogy mely tartományokkal szeretné megosztani a fájlokat:</span><span class="sxs-lookup"><span data-stu-id="f553a-108">In **sharing rule**, select one of the following options to specify the domains you want to share with:</span></span>
    - <span data-ttu-id="f553a-109">**Megosztás az összes tartománysal**</span><span class="sxs-lookup"><span data-stu-id="f553a-109">**Sharing with all domains**</span></span>
    - <span data-ttu-id="f553a-110">**Megosztás egy adott tartománnyal**</span><span class="sxs-lookup"><span data-stu-id="f553a-110">**Sharing with a specific domain**</span></span>
8. <span data-ttu-id="f553a-111">Ha a Megosztás egy adott tartománnyal lehetőséget **választja,** írja be annak a tartománynak a nevét, amelyvel meg szeretné osztani a tartományt.</span><span class="sxs-lookup"><span data-stu-id="f553a-111">If you select **Sharing with a specific domain**, type the name of the domain you want to share with.</span></span> <span data-ttu-id="f553a-112">Ha több tartományt kell megadnia ehhez a megosztási házirendhez, mentse az első tartomány beállításait, majd a megosztási szabályok módosításával vegyen fel további tartományokat.</span><span class="sxs-lookup"><span data-stu-id="f553a-112">If you need to enter more than one domain for this sharing policy, save the settings for the first domain, then edit the sharing rules to add more domains.</span></span>
9. <span data-ttu-id="f553a-113">A megosztható információk megadásához jelölje  be a Naptármappa megosztása jelölőnégyzetet, majd válasszon az alábbi lehetőségek közül:</span><span class="sxs-lookup"><span data-stu-id="f553a-113">To specify the information that can be shared, select the **Share your calendar folder** check box, and then select one of the following options:</span></span>
    - <span data-ttu-id="f553a-114">**Naptár elfoglaltsági adatai csak időponttal**</span><span class="sxs-lookup"><span data-stu-id="f553a-114">**Calendar free/busy information with time only**</span></span>
    - <span data-ttu-id="f553a-115">**Naptár elfoglaltsági adatai időpontmal, témával és helyről**</span><span class="sxs-lookup"><span data-stu-id="f553a-115">**Calendar free/busy information with time, subject, and location**</span></span>
    - <span data-ttu-id="f553a-116">**Minden naptári találkozóra vonatkozó információ, beleértve az időpontot, a tárgyat, a helyet és a címet**</span><span class="sxs-lookup"><span data-stu-id="f553a-116">**All calendar appointment information, including time, subject, location and title**</span></span>
11. <span data-ttu-id="f553a-117">Kattintson **a mentés** gombra a megosztási házirend szabályainak beállításhoz.</span><span class="sxs-lookup"><span data-stu-id="f553a-117">Click **save** to set the rules for the sharing policy.</span></span>
12. <span data-ttu-id="f553a-118">Ha ezt a megosztási házirendet a szervezet minden felhasználója számára új alapértelmezett megosztási házirendként szeretné beállítani, jelölje be a Legyen ez a házirend az alapértelmezett megosztási **házirend** jelölőnégyzetet.</span><span class="sxs-lookup"><span data-stu-id="f553a-118">If you want to set this sharing policy as the new default sharing policy for all users in your organization, select the **Make this policy my default sharing policy** check box.</span></span>
13. <span data-ttu-id="f553a-119">Kattintson **a mentés gombra** a megosztási házirend létrehozásához.</span><span class="sxs-lookup"><span data-stu-id="f553a-119">Click **save** to create the sharing policy.</span></span>  

<span data-ttu-id="f553a-120">**E témakör teljes megértéséhez olvassa el a következő cikket:**</span><span class="sxs-lookup"><span data-stu-id="f553a-120">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="f553a-121">Megosztási házirend létrehozása az Exchange Online-ban</span><span class="sxs-lookup"><span data-stu-id="f553a-121">Create a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/create-a-sharing-policy)
- [<span data-ttu-id="f553a-122">Megosztási házirend alkalmazása postaládákra az Exchange Online-ban</span><span class="sxs-lookup"><span data-stu-id="f553a-122">Apply a sharing policy to mailboxes in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy)
- [<span data-ttu-id="f553a-123">Megosztási házirend módosítása, letiltása vagy eltávolítása az Exchange Online-ban</span><span class="sxs-lookup"><span data-stu-id="f553a-123">Modify, disable, or remove a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)