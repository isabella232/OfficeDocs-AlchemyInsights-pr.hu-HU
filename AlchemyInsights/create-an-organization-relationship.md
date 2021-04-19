---
title: Szervezeti kapcsolat létrehozása, hogy a felhasználók együttműködhetnek egy másik szervezettel
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
ms.openlocfilehash: b595fb87e18a055a7df1ff4c782a93591dd1f024
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816130"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a><span data-ttu-id="144f2-102">Szervezeti kapcsolat létrehozása, hogy a felhasználók együttműködhetnek egy másik szervezettel</span><span class="sxs-lookup"><span data-stu-id="144f2-102">Create an Organization Relationship to allow your users to collaborate with another organization</span></span>

1. <span data-ttu-id="144f2-103">A Microsoft 365 Felügyeleti központ irányítópultján menjen a **Felügyeleti exchange**  >  **lapra.**</span><span class="sxs-lookup"><span data-stu-id="144f2-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="144f2-104">Ugrás a **szervezet**  >  **megosztására .**</span><span class="sxs-lookup"><span data-stu-id="144f2-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="144f2-105">A **Szervezet megosztása alatt kattintson** az Új **elemre.**</span><span class="sxs-lookup"><span data-stu-id="144f2-105">Under **Organization Sharing**, click **New** .</span></span>
4. <span data-ttu-id="144f2-106">Az **új szervezeti kapcsolatokban** a Kapcsolatnév mezőbe írja be a szervezeti kapcsolat rövid nevét. </span><span class="sxs-lookup"><span data-stu-id="144f2-106">In **new organization relationship**, in the **Relationship name** box, type a friendly name for the organization relationship.</span></span>
5. <span data-ttu-id="144f2-107">A **Megosztás a következővel:** tartományok mezőbe írja be annak a külső Office 365-ös vagy helyszíni Exchange-szervezetnek a tartományát, amely a naptárakat meg szeretné osztani.</span><span class="sxs-lookup"><span data-stu-id="144f2-107">In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars.</span></span> <span data-ttu-id="144f2-108">Ha több tartományt kell megadnia, a tartományneveket vesszővel válassza el egymástól.</span><span class="sxs-lookup"><span data-stu-id="144f2-108">If you need to enter more than one domain, separate the domain names with a comma.</span></span> <span data-ttu-id="144f2-109">Például: Contoso.com, service.contoso.com.</span><span class="sxs-lookup"><span data-stu-id="144f2-109">For example, contoso.com, service.contoso.com.</span></span>
6. <span data-ttu-id="144f2-110">Jelölje be **a Naptár foglaltsági adatok megosztásának** engedélyezése jelölőnégyzetet a listában szereplő tartományokkal való naptármegosztás bekapcsolához.</span><span class="sxs-lookup"><span data-stu-id="144f2-110">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed.</span></span> <span data-ttu-id="144f2-111">Állítsa be a naptár foglaltsági információinak megosztási szintjét, és adja meg, hogy mely felhasználók oszthatják meg a naptár foglaltsági adatait.</span><span class="sxs-lookup"><span data-stu-id="144f2-111">Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span></span>  

<span data-ttu-id="144f2-112">A szabad/foglalt hozzáférési szint beállításhoz válasszon az alábbi lehetőségek közül:</span><span class="sxs-lookup"><span data-stu-id="144f2-112">To set the free/busy access level, select one of the following:</span></span>

- <span data-ttu-id="144f2-113">**Naptár elfoglaltsági adatai csak időponttal**</span><span class="sxs-lookup"><span data-stu-id="144f2-113">**Calendar free/busy information with time only**</span></span>
- <span data-ttu-id="144f2-114">**Naptár elfoglaltsági ideje, tárgya és helye**</span><span class="sxs-lookup"><span data-stu-id="144f2-114">**Calendar free/busy with time, subject, and location**</span></span>  

 <span data-ttu-id="144f2-115">Ha azt adja meg, hogy mely felhasználók osztanának meg naptár foglaltsági adatokat, válasszon az alábbi lehetőségek közül:</span><span class="sxs-lookup"><span data-stu-id="144f2-115">To set which users will share calendar free/busy information, select one of the following:</span></span>

- <span data-ttu-id="144f2-116">**A szervezet minden tagja**</span><span class="sxs-lookup"><span data-stu-id="144f2-116">**Everyone in your organization**</span></span>
- <span data-ttu-id="144f2-117">**Egy megadott biztonsági csoport**</span><span class="sxs-lookup"><span data-stu-id="144f2-117">**A specified security group**</span></span>  

<span data-ttu-id="144f2-118">Kattintson **a tallózás** gombra a biztonsági csoport listából való választásához, majd kattintson az ok **gombra.**</span><span class="sxs-lookup"><span data-stu-id="144f2-118">Click **browse** to pick the security group from a list, then click **ok**.</span></span>

<span data-ttu-id="144f2-119">Kattintson **a mentés** gombra a szervezeti kapcsolat létrehozásához.</span><span class="sxs-lookup"><span data-stu-id="144f2-119">Click **save** to create the organization relationship.</span></span>  

<span data-ttu-id="144f2-120">**Megjegyzés:** A több-bérlős konfigurációk nem támogatják a személyes névjegyeket az elfoglalt/foglalt kereséshez.</span><span class="sxs-lookup"><span data-stu-id="144f2-120">**Note:** Cross-tenant configurations do not support personal contacts for free/busy lookup.</span></span> <span data-ttu-id="144f2-121">A partnereknek szerepelniük kell a globális címlistában ahhoz, hogy a foglalt/foglalt keresés működjön.</span><span class="sxs-lookup"><span data-stu-id="144f2-121">Contacts must be included in the global address list for free/busy lookup to work.</span></span>

<span data-ttu-id="144f2-122">**E témakör teljes megértéséhez olvassa el a következő cikket:**</span><span class="sxs-lookup"><span data-stu-id="144f2-122">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="144f2-123">Szervezeti kapcsolat létrehozása az Exchange Online-ban</span><span class="sxs-lookup"><span data-stu-id="144f2-123">Create an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [<span data-ttu-id="144f2-124">Szervezeti kapcsolat módosítása az Exchange Online-ban</span><span class="sxs-lookup"><span data-stu-id="144f2-124">Modify an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [<span data-ttu-id="144f2-125">Szervezeti kapcsolat eltávolítása az Exchange Online-ban</span><span class="sxs-lookup"><span data-stu-id="144f2-125">Remove an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
