---
title: Külső felhasználók hozzáadása a terjesztési csoporthoz
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 641636add2069fc395df9af156d8c011493a634a
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/29/2019
ms.locfileid: "36660794"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="53625-102">Külső felhasználók hozzáadása terjesztési csoporthoz</span><span class="sxs-lookup"><span data-stu-id="53625-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="53625-103">A terjesztési csoporthoz (DG) külső kapcsolattartó hozzáadása két lépésben történik:</span><span class="sxs-lookup"><span data-stu-id="53625-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="53625-104">Levelezési kapcsolat létrehozása a külső felhasználó számára:</span><span class="sxs-lookup"><span data-stu-id="53625-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="53625-105">Az admin központban lépjen a **felhasználók** > [névjegyalbumoldalára](https://admin.microsoft.com/adminportal/home#/Contact) .</span><span class="sxs-lookup"><span data-stu-id="53625-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="53625-106">Válassza **a Névjegy hozzáadása**-t.</span><span class="sxs-lookup"><span data-stu-id="53625-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="53625-107">Írja be a névjegyhez tartozó adatokat, és válassza a **hozzáad**-t.</span><span class="sxs-lookup"><span data-stu-id="53625-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="53625-108">A levelezési kapcsolat felvétele a FŐIGAZGATÓSÁGBA:</span><span class="sxs-lookup"><span data-stu-id="53625-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="53625-109">Az admin központban lépjen a **csoportok** > [csoportjai](https://admin.microsoft.com/adminportal/home#/groups) oldalra.</span><span class="sxs-lookup"><span data-stu-id="53625-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="53625-110">Keresse meg azt a FŐIGAZGATÓSÁGOT, amelyhez hozzá szeretné adni a külső felhasználót, majd jelölje ki a szerkesztési párbeszédpanel megnyitásához.</span><span class="sxs-lookup"><span data-stu-id="53625-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="53625-111">A **tagok** lapon jelölje be az **összes megtekintése és a tagok kezelése**választógombot.</span><span class="sxs-lookup"><span data-stu-id="53625-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="53625-112">Válassza a **Tagok felvétele**-t.</span><span class="sxs-lookup"><span data-stu-id="53625-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="53625-113">Válassza ki az előző lépésben létrehozott levelezési névjegyet, majd válassza a **Mentés**-t.</span><span class="sxs-lookup"><span data-stu-id="53625-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="53625-114">Ha a következő lépések megtételét követően a külső felhasználók nem tudnak e-maileket küldeni a DG-nek, vagy nem kapnak e-maileket, akkor lehet, hogy a FŐIGAZGATÓSÁGNAK csak belső felhasználóktól származó leveleket enged meg.</span><span class="sxs-lookup"><span data-stu-id="53625-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="53625-115">Tudod ellenőriz ez alakzat és erősít ez alábbiak a utasítások [itt](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).</span><span class="sxs-lookup"><span data-stu-id="53625-115">You can check this configuration and fix it following the directions [here](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx).</span></span>
  
 <span data-ttu-id="53625-116">**Megjegyzés:** Ezek az utasítások nem alkalmazhatók, ha a csoport típusa "terjesztési csoport" helyett "Office 365 csoport".</span><span class="sxs-lookup"><span data-stu-id="53625-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="53625-117">Ebben az esetben a külső felhasználót közvetlenül is hozzáadhatja a csoporthoz az Outlook programból.</span><span class="sxs-lookup"><span data-stu-id="53625-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="53625-118">Részletes információ az Office 365 csoportokról, a vendégek és a külső vendégek hozzáadására vonatkozó utasítások megtalálhatók [ebben a cikkben](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="53625-118">Detailed information on Office 365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  