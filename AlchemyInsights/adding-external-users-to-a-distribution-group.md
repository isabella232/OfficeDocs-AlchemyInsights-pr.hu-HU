---
title: Terjesztési csoport külső felhasználó hozzáadása
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 8/22/2017
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: ce0c589e1661fb4607452fe2e8f897758b2718e8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36494529"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="2e504-102">Külső felhasználók hozzáadása a terjesztési csoportot?</span><span class="sxs-lookup"><span data-stu-id="2e504-102">Add external users to a Distribution Group?</span></span>

<span data-ttu-id="2e504-103">Hozzáadása egy külső partner, a terjesztési csoport (DG) egy 2 lépésből álló folyamat:</span><span class="sxs-lookup"><span data-stu-id="2e504-103">Adding an external contact to a Distribution Group (DG) is a 2-step process:</span></span>
  
1. <span data-ttu-id="2e504-104">A külső felhasználó levelezési névjegy létrehozása:</span><span class="sxs-lookup"><span data-stu-id="2e504-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="2e504-105">A felügyeleti központ, keresse meg a **felhasználók** > [Névjegyalbum](https://admin.microsoft.com/adminportal/home#/Contact) lapon.</span><span class="sxs-lookup"><span data-stu-id="2e504-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="2e504-106">Válassza ki a **Partner felvétele**.</span><span class="sxs-lookup"><span data-stu-id="2e504-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="2e504-107">Írja be a partner adatait, és válassza a **Hozzáadás gombra**.</span><span class="sxs-lookup"><span data-stu-id="2e504-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="2e504-108">Adja hozzá a levél az ügyfélnek a DG:</span><span class="sxs-lookup"><span data-stu-id="2e504-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="2e504-109">A **csoportok**Ugrás az admin center > [csoportok](https://admin.microsoft.com/adminportal/home#/groups) lapon.</span><span class="sxs-lookup"><span data-stu-id="2e504-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="2e504-110">Keresse meg a DG szeretne hozzáadni a külső felhasználó, és jelölje ki azt a Szerkesztés párbeszédpanel megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="2e504-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="2e504-111">A **tagok** lapon jelölje be **az összes megtekintése és kezelése a tagok**.</span><span class="sxs-lookup"><span data-stu-id="2e504-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="2e504-112">Válassza ki a **Tagok hozzáadása**.</span><span class="sxs-lookup"><span data-stu-id="2e504-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="2e504-113">Válassza ki az előző lépésben létrehozott levelezési ügyfelet, és válassza a **Mentés**.</span><span class="sxs-lookup"><span data-stu-id="2e504-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="2e504-114">Ha ezen lépések után a külső felhasználók nem küldhet e-maileket a DG, vagy nem kap e-mailek belőle, lehet, hogy a DG e-mailek engedélyezése csak a belső felhasználók számára van megjelölve.</span><span class="sxs-lookup"><span data-stu-id="2e504-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="2e504-115">Ellenőrizze a konfigurációt, és javítsa ki a következő utasításokat [Itt](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).</span><span class="sxs-lookup"><span data-stu-id="2e504-115">You can check this configuration and fix it following the directions [here](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).</span></span>
  
 <span data-ttu-id="2e504-116">**Megjegyzés:** Ezeket az utasításokat nem alkalmazhatók, ha a csoport típusa "Office 365-csoport" helyett "Terjesztési csoport."</span><span class="sxs-lookup"><span data-stu-id="2e504-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="2e504-117">Ha ez az eset, hozzáadhatja a külső felhasználó közvetlenül a csoport az Outlook programból.</span><span class="sxs-lookup"><span data-stu-id="2e504-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="2e504-118">Office 365 csoportok vendégek részletes tájékoztatást és utasításokat külső Vendégek hozzáadása a [cikkben](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)található.</span><span class="sxs-lookup"><span data-stu-id="2e504-118">Detailed information on Office 365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  