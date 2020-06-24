---
title: Szervezeti kapcsolat létrehozása, amely lehetővé teszi a felhasználók számára, hogy együttműködjenek egy másik szervezettel
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
ms.openlocfilehash: 2c6cd6a178c6e012bfe1c8d769b037168ffa3254
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862106"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a><span data-ttu-id="38a6e-102">Szervezeti kapcsolat létrehozása, amely lehetővé teszi a felhasználók számára, hogy együttműködjenek egy másik szervezettel</span><span class="sxs-lookup"><span data-stu-id="38a6e-102">Create an Organization Relationship to allow your users to collaborate with another organization</span></span>

1. <span data-ttu-id="38a6e-103">A Microsoft 365 Felügyeleti központ irányítópultjáról nyissa meg a **Admin**  >  **Exchange**lapot.</span><span class="sxs-lookup"><span data-stu-id="38a6e-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="38a6e-104">Nyissa **organization**meg a  >  **szervezetmegosztást.**</span><span class="sxs-lookup"><span data-stu-id="38a6e-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="38a6e-105">A **Szervezeti megosztás csoportban**kattintson az **Új** gombra.</span><span class="sxs-lookup"><span data-stu-id="38a6e-105">Under **Organization Sharing**, click **New** .</span></span>
4. <span data-ttu-id="38a6e-106">Az **új szervezeti kapcsolat**mezőbe írja be a szervezeti kapcsolat rövid nevét. **Relationship name**</span><span class="sxs-lookup"><span data-stu-id="38a6e-106">In **new organization relationship**, in the **Relationship name** box, type a friendly name for the organization relationship.</span></span>
5. <span data-ttu-id="38a6e-107">A **Megosztani kívánt tartományok** mezőbe írja be annak a külső Office 365-nek vagy az Exchange helyszíni szervezetnek a tartományát, amelyet látni szeretne a naptáraiban.</span><span class="sxs-lookup"><span data-stu-id="38a6e-107">In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars.</span></span> <span data-ttu-id="38a6e-108">Ha egynél több tartományt kell megadnia, válassza el a tartományneveket vesszővel.</span><span class="sxs-lookup"><span data-stu-id="38a6e-108">If you need to enter more than one domain, separate the domain names with a comma.</span></span> <span data-ttu-id="38a6e-109">Például contoso.com, service.contoso.com.</span><span class="sxs-lookup"><span data-stu-id="38a6e-109">For example, contoso.com, service.contoso.com.</span></span>
6. <span data-ttu-id="38a6e-110">Jelölje be a **Naptár elfoglaltsági adatainak megosztásának engedélyezése** jelölőnégyzetet, ha be szeretné kapcsolni a naptármegosztást a felsorolt tartományokkal.</span><span class="sxs-lookup"><span data-stu-id="38a6e-110">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed.</span></span> <span data-ttu-id="38a6e-111">Állítsa be a naptár elfoglaltsági adatainak megosztási szintjét, és azt, hogy a felhasználók mely elfoglaltsági adatokat oszthatják meg.</span><span class="sxs-lookup"><span data-stu-id="38a6e-111">Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span></span>  

<span data-ttu-id="38a6e-112">Az elfoglaltsági szint beállításához válasszon az alábbi feltételek közül:</span><span class="sxs-lookup"><span data-stu-id="38a6e-112">To set the free/busy access level, select one of the following:</span></span>

- <span data-ttu-id="38a6e-113">**Naptár elfoglaltsági adatai csak időponttal**</span><span class="sxs-lookup"><span data-stu-id="38a6e-113">**Calendar free/busy information with time only**</span></span>
- <span data-ttu-id="38a6e-114">**Naptár elfoglaltsága az idővel, a témával és a helynel**</span><span class="sxs-lookup"><span data-stu-id="38a6e-114">**Calendar free/busy with time, subject, and location**</span></span>  

 <span data-ttu-id="38a6e-115">Annak beállításához, hogy mely felhasználók osszák meg a naptár elfoglaltsági adatait, válasszon az alábbi adatok közül:</span><span class="sxs-lookup"><span data-stu-id="38a6e-115">To set which users will share calendar free/busy information, select one of the following:</span></span>

- <span data-ttu-id="38a6e-116">**A szervezet minden tagja**</span><span class="sxs-lookup"><span data-stu-id="38a6e-116">**Everyone in your organization**</span></span>
- <span data-ttu-id="38a6e-117">**Egy megadott biztonsági csoport**</span><span class="sxs-lookup"><span data-stu-id="38a6e-117">**A specified security group**</span></span>  

<span data-ttu-id="38a6e-118">A **Tallózás gombra** kattintva válassza ki a biztonsági csoportot a listából, majd kattintson az **OK gombra.**</span><span class="sxs-lookup"><span data-stu-id="38a6e-118">Click **browse** to pick the security group from a list, then click **ok**.</span></span>

<span data-ttu-id="38a6e-119">Kattintson a **Mentés** gombra a szervezeti kapcsolat létrehozásához.</span><span class="sxs-lookup"><span data-stu-id="38a6e-119">Click **save** to create the organization relationship.</span></span>  

<span data-ttu-id="38a6e-120">**Megjegyzés:** A bérlők közötti konfigurációk nem támogatják a személyes kapcsolatokat az elfoglaltsági adatok keresése érdekében.</span><span class="sxs-lookup"><span data-stu-id="38a6e-120">**Note:** Cross-tenant configurations do not support personal contacts for free/busy lookup.</span></span> <span data-ttu-id="38a6e-121">Az elfoglaltsági/munkabe( foglaltság) globális címlistájában fel kell venni a névjegyeket.</span><span class="sxs-lookup"><span data-stu-id="38a6e-121">Contacts must be included in the global address list for free/busy lookup to work.</span></span>

<span data-ttu-id="38a6e-122">**A teljes megértéséhez ezt a témát kérjük, olvassa el:**</span><span class="sxs-lookup"><span data-stu-id="38a6e-122">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="38a6e-123">Szervezeti kapcsolat létrehozása az Exchange Online-ban</span><span class="sxs-lookup"><span data-stu-id="38a6e-123">Create an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [<span data-ttu-id="38a6e-124">Szervezeti kapcsolat módosítása az Exchange Online-ban</span><span class="sxs-lookup"><span data-stu-id="38a6e-124">Modify an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [<span data-ttu-id="38a6e-125">Szervezeti kapcsolat eltávolítása az Exchange Online-ban</span><span class="sxs-lookup"><span data-stu-id="38a6e-125">Remove an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
