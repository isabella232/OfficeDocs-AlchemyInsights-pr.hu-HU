---
title: Az IP-videó engedélyezése vagy letiltása a Teamsben
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
- "9002537"
- "5617"
ms.openlocfilehash: 059d7a1ad619e25f14bc6f561693b6fe24355132
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826345"
---
# <a name="teams-allow-or-disable-ip-video"></a><span data-ttu-id="27a5f-102">Az IP-videó engedélyezése vagy letiltása a Teamsben</span><span class="sxs-lookup"><span data-stu-id="27a5f-102">Teams allow or disable IP video</span></span>

<span data-ttu-id="27a5f-103">**Értekezleti házirend módosítása vagy létrehozása**</span><span class="sxs-lookup"><span data-stu-id="27a5f-103">**Change or create a meeting policy**</span></span>

<span data-ttu-id="27a5f-104">Értekezleti házirendek módosítása vagy létrehozása: A Microsoft Teams Felügyeleti **központ értekezletek > értekezleti > értekezleti házirendek .**</span><span class="sxs-lookup"><span data-stu-id="27a5f-104">To change or create a meeting policy, go to the **Microsoft Teams admin center > Meetings > Meeting policies**.</span></span> <span data-ttu-id="27a5f-105">Válasszon egy szabályzatot a listából, vagy válassza a **Hozzáadás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="27a5f-105">Select a policy from the list or click **Add**.</span></span> <span data-ttu-id="27a5f-106">Ha új szabályzatot hoz létre, adja meg a nevét és a leírását.</span><span class="sxs-lookup"><span data-stu-id="27a5f-106">If you're creating a new policy, add a name and description.</span></span> <span data-ttu-id="27a5f-107">A név nem tartalmazhat speciális karaktereket, és nem lehet hosszabb 64 karakternél.</span><span class="sxs-lookup"><span data-stu-id="27a5f-107">The name can't contain special characters or be longer than 64 characters.</span></span> <span data-ttu-id="27a5f-108">Adja meg a kívánt beállításokat, majd kattintson a **Mentés** gombra.</span><span class="sxs-lookup"><span data-stu-id="27a5f-108">Choose your settings, and then click **Save**.</span></span>

<span data-ttu-id="27a5f-109">Tegyük fel például, hogy sok felhasználója van, és korlátozni szeretné az értekezlethez szükséges sávszélességet.</span><span class="sxs-lookup"><span data-stu-id="27a5f-109">For example, say you have many users and you want to limit the amount of bandwidth that their meeting would require.</span></span> <span data-ttu-id="27a5f-110">Érdemes létrehoznia egy „Korlátozott sávszélesség” nevű új szabályzatot és letiltani a következő beállításokat:</span><span class="sxs-lookup"><span data-stu-id="27a5f-110">You would create a new custom policy named "Limited bandwidth" and disable the following settings:</span></span>

<span data-ttu-id="27a5f-111">A **Hang és videó** csoportban:</span><span class="sxs-lookup"><span data-stu-id="27a5f-111">Under **Audio & video**:</span></span>

- <span data-ttu-id="27a5f-112">Kapcsolja ki a Felhőalapú rögzítés engedélyezése beállítást.</span><span class="sxs-lookup"><span data-stu-id="27a5f-112">Turn off Allow cloud recording.</span></span>
- <span data-ttu-id="27a5f-113">Kapcsolja ki az IP-videó engedélyezése beállítást.</span><span class="sxs-lookup"><span data-stu-id="27a5f-113">Turn off Allow IP video.</span></span>

<span data-ttu-id="27a5f-114">Ezután rendelje hozzá a szabályzatot a felhasználókhoz.</span><span class="sxs-lookup"><span data-stu-id="27a5f-114">Then assign the policy to the users.</span></span>

<span data-ttu-id="27a5f-115">**Értekezletszabályzat hozzárendelése felhasználókhoz**</span><span class="sxs-lookup"><span data-stu-id="27a5f-115">**Assign a meeting policy to users**</span></span>

1. <span data-ttu-id="27a5f-116">A Microsoft Teams Felügyeleti központ bal oldali navigációs panelén keresse meg a **Felhasználók** lehetőséget, és kattintson a felhasználóra.</span><span class="sxs-lookup"><span data-stu-id="27a5f-116">In the left navigation of the Microsoft Teams admin center, go to **Users**, and then click the user.</span></span>
2. <span data-ttu-id="27a5f-117">A felhasználónévtől balra kattintva jelölje ki a felhasználót, és kattintson a **Beállítások szerkesztése** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="27a5f-117">Select the user by clicking to the left of the user name, and then click **Edit settings**.</span></span>
3. <span data-ttu-id="27a5f-118">Az **Értekezleti házirend alatt** válassza ki a hozzárendelni kívánt házirendet, majd kattintson az Alkalmaz **gombra.**</span><span class="sxs-lookup"><span data-stu-id="27a5f-118">Under **Meeting policy**, select the policy you want to assign and then click **Apply**.</span></span>

<span data-ttu-id="27a5f-119">További információ: Értekezleti [házirendek kezelése a Teamsben.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="27a5f-119">For more information, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>
