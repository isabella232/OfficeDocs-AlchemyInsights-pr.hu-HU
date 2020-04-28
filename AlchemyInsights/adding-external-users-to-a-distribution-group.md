---
title: Külső felhasználók hozzáadása terjesztési csoporthoz
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 7dbc69bced9ca800d3f95081b77dda5e49662579
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/27/2020
ms.locfileid: "43910934"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="d05e6-102">Külső felhasználók hozzáadása terjesztési csoporthoz</span><span class="sxs-lookup"><span data-stu-id="d05e6-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="d05e6-103">Külső kapcsolattartó hozzáadása egy terjesztési csoporthoz két lépésből áll:</span><span class="sxs-lookup"><span data-stu-id="d05e6-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="d05e6-104">E-mail névjegy létrehozása a külső felhasználó számára:</span><span class="sxs-lookup"><span data-stu-id="d05e6-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="d05e6-105">A felügyeleti központban nyissa meg a **Felhasználók névjegyei** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) lapot.</span><span class="sxs-lookup"><span data-stu-id="d05e6-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="d05e6-106">Válassza **a Partner hozzáadása**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="d05e6-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="d05e6-107">Írja be a partner adatait, és válassza a **Hozzáadás gombot.**</span><span class="sxs-lookup"><span data-stu-id="d05e6-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="d05e6-108">A Levelezési kapcsolattartó felvétele a főigazgatósághoz:</span><span class="sxs-lookup"><span data-stu-id="d05e6-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="d05e6-109">A felügyeleti központban nyissa meg a **Csoportok** > [csoportját.](https://admin.microsoft.com/adminportal/home#/groups)</span><span class="sxs-lookup"><span data-stu-id="d05e6-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="d05e6-110">Keresse meg azt a főigazgatóságot, amelyhez hozzá szeretné adni a külső felhasználót, és jelölje ki a szerkesztési párbeszédpanel megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="d05e6-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="d05e6-111">A **Tagok** lapon válassza az **Összes megtekintése és a tagok kezelése**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="d05e6-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="d05e6-112">Válassza **a Tagok hozzáadása**lehetőséget.</span><span class="sxs-lookup"><span data-stu-id="d05e6-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="d05e6-113">Jelölje ki az előző lépésben létrehozott Levelezési névjegyet, majd kattintson a **Mentés gombra.**</span><span class="sxs-lookup"><span data-stu-id="d05e6-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="d05e6-114">Ha e lépések bekövetése után a külső felhasználók nem tudnak e-maileket küldeni a főigazgatóságnak, vagy nem kapnak tőle e-maileket, akkor előfordulhat, hogy a főigazgatóság csak a belső felhasználóktól származó e-maileket engedélyezi.</span><span class="sxs-lookup"><span data-stu-id="d05e6-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="d05e6-115">Tudod ellenőriz ez alakzat és erősít ez alábbiak a utasítások [itt.](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)</span><span class="sxs-lookup"><span data-stu-id="d05e6-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="d05e6-116">**Megjegyzés:** Ezek az utasítások nem érvényesek, ha a csoport típusa "Microsoft 365 csoport" a "Terjesztési csoport" helyett.</span><span class="sxs-lookup"><span data-stu-id="d05e6-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="d05e6-117">Ebben az esetben a külső felhasználót közvetlenül is hozzáadhatja a csoporthoz az Outlook programból.</span><span class="sxs-lookup"><span data-stu-id="d05e6-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="d05e6-118">A Microsoft 365 Csoportok vendégeiről, valamint a külső vendégek hozzáadására vonatkozó utasításokról ebben a cikkben olvashat [részletesen.](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)</span><span class="sxs-lookup"><span data-stu-id="d05e6-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  