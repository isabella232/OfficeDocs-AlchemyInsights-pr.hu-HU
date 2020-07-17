---
title: Megosztási szabályzat létrehozása, amely lehetővé teszi a felhasználók számára, hogy megosszák naptárukat a szervezeten kívüli emberekkel
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: cb2c0af55f4f8833709b6952d3a6e2ac258ce5fc
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862115"
---
# <a name="create-a-sharing-policy-to-allow-your-users-to-share-their-calendar-with-people-outside-your-organization"></a><span data-ttu-id="8cc7d-102">Megosztási szabályzat létrehozása, amely lehetővé teszi a felhasználók számára, hogy megosszák naptárukat a szervezeten kívüli emberekkel</span><span class="sxs-lookup"><span data-stu-id="8cc7d-102">Create a Sharing Policy to allow your users to share their calendar with people outside your organization</span></span>

1. <span data-ttu-id="8cc7d-103">A Microsoft 365 Felügyeleti központ irányítópultjáról nyissa meg a **Admin**  >  **Exchange**lapot.</span><span class="sxs-lookup"><span data-stu-id="8cc7d-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="8cc7d-104">Nyissa **organization**meg a  >  **szervezetmegosztást.**</span><span class="sxs-lookup"><span data-stu-id="8cc7d-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="8cc7d-105">A listanézetEgyéni megosztás csoportban kattintson az **Új** **gombra.**</span><span class="sxs-lookup"><span data-stu-id="8cc7d-105">In the list view, under **Individual Sharing**, click **New** .</span></span>
4. <span data-ttu-id="8cc7d-106">Az **új megosztási házirendben**írja be a megosztási házirend rövid nevét a **Házirend neve** mezőbe.</span><span class="sxs-lookup"><span data-stu-id="8cc7d-106">In **new sharing policy**, type a friendly name for the sharing policy in the **Policy name** box.</span></span>
5. <span data-ttu-id="8cc7d-107">Kattintson a **Hozzáadás** gombra a házirend megosztási szabályainak meghatározásához.</span><span class="sxs-lookup"><span data-stu-id="8cc7d-107">Click **Add**  to define the sharing rules for the policy.</span></span>
6. <span data-ttu-id="8cc7d-108">A **megosztási szabályban**válasszon az alábbi lehetőségek közül, hogy megadja azokat a tartományokat, amelyekkel meg szeretné osztani a kívánt tartományokat:</span><span class="sxs-lookup"><span data-stu-id="8cc7d-108">In **sharing rule**, select one of the following options to specify the domains you want to share with:</span></span>
    - <span data-ttu-id="8cc7d-109">**Megosztás az összes tartománnyal**</span><span class="sxs-lookup"><span data-stu-id="8cc7d-109">**Sharing with all domains**</span></span>
    - <span data-ttu-id="8cc7d-110">**Megosztás egy adott tartománnyal**</span><span class="sxs-lookup"><span data-stu-id="8cc7d-110">**Sharing with a specific domain**</span></span>
8. <span data-ttu-id="8cc7d-111">Ha **a Megosztás egy adott tartománnyal lehetőséget választja,** írja be annak a tartománynak a nevét, amelyet meg szeretne osztani.</span><span class="sxs-lookup"><span data-stu-id="8cc7d-111">If you select **Sharing with a specific domain**, type the name of the domain you want to share with.</span></span> <span data-ttu-id="8cc7d-112">Ha egynél több tartományt kell megadnia ehhez a megosztási házirendhez, mentse az első tartomány beállításait, majd a megosztási szabályok szerkesztésével adjon hozzá további tartományokat.</span><span class="sxs-lookup"><span data-stu-id="8cc7d-112">If you need to enter more than one domain for this sharing policy, save the settings for the first domain, then edit the sharing rules to add more domains.</span></span>
9. <span data-ttu-id="8cc7d-113">A megosztható adatok megadásához jelölje be a **Naptármappa megosztása jelölőnégyzetet,** majd válasszon az alábbi lehetőségek közül:</span><span class="sxs-lookup"><span data-stu-id="8cc7d-113">To specify the information that can be shared, select the **Share your calendar folder** check box, and then select one of the following options:</span></span>
    - <span data-ttu-id="8cc7d-114">**Naptár elfoglaltsági adatai csak időponttal**</span><span class="sxs-lookup"><span data-stu-id="8cc7d-114">**Calendar free/busy information with time only**</span></span>
    - <span data-ttu-id="8cc7d-115">**Naptár elfoglaltsági adatai az idővel, a témával és a helynel**</span><span class="sxs-lookup"><span data-stu-id="8cc7d-115">**Calendar free/busy information with time, subject, and location**</span></span>
    - <span data-ttu-id="8cc7d-116">**A naptár minden találkozójának információja, beleértve az időt, a tárgyat, a helyet és a címet**</span><span class="sxs-lookup"><span data-stu-id="8cc7d-116">**All calendar appointment information, including time, subject, location and title**</span></span>
11. <span data-ttu-id="8cc7d-117">Kattintson a **Mentés** gombra a megosztási házirend szabályainak beállításához.</span><span class="sxs-lookup"><span data-stu-id="8cc7d-117">Click **save** to set the rules for the sharing policy.</span></span>
12. <span data-ttu-id="8cc7d-118">Ha ezt a megosztási házirendet szeretné a szervezet összes felhasználója új alapértelmezett megosztási házirendjeként beállítani, jelölje be a Házirend legyen **az alapértelmezett megosztási házirendje** jelölőnégyzetet.</span><span class="sxs-lookup"><span data-stu-id="8cc7d-118">If you want to set this sharing policy as the new default sharing policy for all users in your organization, select the **Make this policy my default sharing policy** check box.</span></span>
13. <span data-ttu-id="8cc7d-119">Kattintson a **Mentés** gombra a megosztási házirend létrehozásához.</span><span class="sxs-lookup"><span data-stu-id="8cc7d-119">Click **save** to create the sharing policy.</span></span>  

<span data-ttu-id="8cc7d-120">**A teljes megértéséhez ezt a témát kérjük, olvassa el:**</span><span class="sxs-lookup"><span data-stu-id="8cc7d-120">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="8cc7d-121">Megosztási házirend létrehozása az Exchange Online-ban</span><span class="sxs-lookup"><span data-stu-id="8cc7d-121">Create a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/create-a-sharing-policy)
- [<span data-ttu-id="8cc7d-122">Megosztási házirend alkalmazása postaládákra az Exchange Online-ban</span><span class="sxs-lookup"><span data-stu-id="8cc7d-122">Apply a sharing policy to mailboxes in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy)
- [<span data-ttu-id="8cc7d-123">Megosztási házirend módosítása, letiltása vagy eltávolítása az Exchange Online-ban</span><span class="sxs-lookup"><span data-stu-id="8cc7d-123">Modify, disable, or remove a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)