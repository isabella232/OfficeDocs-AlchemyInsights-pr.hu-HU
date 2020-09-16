---
title: Az IP-videó engedélyezése vagy letiltása a csoportokban
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002537"
- "5617"
ms.openlocfilehash: cf2d67170f846db1d5d2f1ca8c8b50902e200e45
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670186"
---
# <a name="teams-allow-or-disable-ip-video"></a><span data-ttu-id="541cc-102">Az IP-videó engedélyezése vagy letiltása a csoportokban</span><span class="sxs-lookup"><span data-stu-id="541cc-102">Teams allow or disable IP video</span></span>

<span data-ttu-id="541cc-103">**Értekezlet-házirend módosítása vagy létrehozása**</span><span class="sxs-lookup"><span data-stu-id="541cc-103">**Change or create a meeting policy**</span></span>

<span data-ttu-id="541cc-104">Az értekezlet-összehívások módosításához vagy létrehozásához nyissa meg a **Microsoft Teams felügyeleti központot > értekezletek > értekezlet-házirendeket**.</span><span class="sxs-lookup"><span data-stu-id="541cc-104">To change or create a meeting policy, go to the **Microsoft Teams admin center > Meetings > Meeting policies**.</span></span> <span data-ttu-id="541cc-105">Válasszon egy szabályzatot a listából, vagy válassza a **Hozzáadás** lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="541cc-105">Select a policy from the list or click **Add**.</span></span> <span data-ttu-id="541cc-106">Ha új szabályzatot hoz létre, adja meg a nevét és a leírását.</span><span class="sxs-lookup"><span data-stu-id="541cc-106">If you're creating a new policy, add a name and description.</span></span> <span data-ttu-id="541cc-107">A név nem tartalmazhat speciális karaktereket, és nem lehet hosszabb 64 karakternél.</span><span class="sxs-lookup"><span data-stu-id="541cc-107">The name can't contain special characters or be longer than 64 characters.</span></span> <span data-ttu-id="541cc-108">Adja meg a kívánt beállításokat, majd kattintson a **Mentés** gombra.</span><span class="sxs-lookup"><span data-stu-id="541cc-108">Choose your settings, and then click **Save**.</span></span>

<span data-ttu-id="541cc-109">Tegyük fel például, hogy sok felhasználója van, és korlátozni szeretné az értekezlethez szükséges sávszélesség mértékét.</span><span class="sxs-lookup"><span data-stu-id="541cc-109">For example, say you have many users and you want to limit the amount of bandwidth that their meeting would require.</span></span> <span data-ttu-id="541cc-110">Érdemes létrehoznia egy „Korlátozott sávszélesség” nevű új szabályzatot és letiltani a következő beállításokat:</span><span class="sxs-lookup"><span data-stu-id="541cc-110">You would create a new custom policy named "Limited bandwidth" and disable the following settings:</span></span>

<span data-ttu-id="541cc-111">A **Hang és videó** csoportban:</span><span class="sxs-lookup"><span data-stu-id="541cc-111">Under **Audio & video**:</span></span>

- <span data-ttu-id="541cc-112">Kapcsolja ki a Felhőalapú rögzítés engedélyezése beállítást.</span><span class="sxs-lookup"><span data-stu-id="541cc-112">Turn off Allow cloud recording.</span></span>
- <span data-ttu-id="541cc-113">Kapcsolja ki az IP-videó engedélyezése beállítást.</span><span class="sxs-lookup"><span data-stu-id="541cc-113">Turn off Allow IP video.</span></span>

<span data-ttu-id="541cc-114">Ezután rendelje hozzá a szabályzatot a felhasználókhoz.</span><span class="sxs-lookup"><span data-stu-id="541cc-114">Then assign the policy to the users.</span></span>

<span data-ttu-id="541cc-115">**Értekezletszabályzat hozzárendelése felhasználókhoz**</span><span class="sxs-lookup"><span data-stu-id="541cc-115">**Assign a meeting policy to users**</span></span>

1. <span data-ttu-id="541cc-116">A Microsoft Teams Felügyeleti központ bal oldali navigációs panelén keresse meg a **Felhasználók** lehetőséget, és kattintson a felhasználóra.</span><span class="sxs-lookup"><span data-stu-id="541cc-116">In the left navigation of the Microsoft Teams admin center, go to **Users**, and then click the user.</span></span>
2. <span data-ttu-id="541cc-117">A felhasználónévtől balra kattintva jelölje ki a felhasználót, és kattintson a **Beállítások szerkesztése** lehetőségre.</span><span class="sxs-lookup"><span data-stu-id="541cc-117">Select the user by clicking to the left of the user name, and then click **Edit settings**.</span></span>
3. <span data-ttu-id="541cc-118">Az **értekezlet-házirend**csoportban jelölje ki a hozzárendelni kívánt házirendet, majd kattintson az **alkalmaz**gombra.</span><span class="sxs-lookup"><span data-stu-id="541cc-118">Under **Meeting policy**, select the policy you want to assign and then click **Apply**.</span></span>

<span data-ttu-id="541cc-119">További információt az [értekezlet-házirendek kezelése a Teams alkalmazásban](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="541cc-119">For more information, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>
