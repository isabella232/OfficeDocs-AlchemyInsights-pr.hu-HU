---
title: Csapatok privát csatornájának törlése
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439326"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="01abe-102">Csapatok privát csatornájának törlése</span><span class="sxs-lookup"><span data-stu-id="01abe-102">Delete a Teams private channel</span></span>

<span data-ttu-id="01abe-103">A Microsoft nak tudomása van arról, hogy probléma van a Teams privát csatornáinak törlésével, ha az alapul szolgáló SharePoint-webhelyhez engedélyezve van a SharePoint-adatmegőrzési házirendek.</span><span class="sxs-lookup"><span data-stu-id="01abe-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="01abe-104">A Microsoft dolgozik egy javításon.</span><span class="sxs-lookup"><span data-stu-id="01abe-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="01abe-105">Addig is a következő kerülő megoldások segítségével törölheti a privát csatornát.</span><span class="sxs-lookup"><span data-stu-id="01abe-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="01abe-106">**A csoport-/webhelycsoport kizárása a SharePoint-adatmegőrzési szabályból.**</span><span class="sxs-lookup"><span data-stu-id="01abe-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="01abe-107">Nyissa meg az Office 365 felügyeleti portálját, és válassza az **Összes megjelenítése** lehetőséget a bal oldali navigációs ablakban.</span><span class="sxs-lookup"><span data-stu-id="01abe-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="01abe-108">A **Felügyeleti központok csoportban**nyissa meg **a Biztonsági &**  >  **megfelelőségi adatveszteség-megelőzési**  >  **házirendet.**</span><span class="sxs-lookup"><span data-stu-id="01abe-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="01abe-109">Azonosítsa a SharePoint-webhelyekre vonatkozó házirendeket, és módosítsa a házirendet úgy, hogy a privát csatornát tartalmazó csoport SharePoint-webhelye NE szerepeljen az adatmegőrzési szabályzatban.</span><span class="sxs-lookup"><span data-stu-id="01abe-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="01abe-110">Mentse a házirendet.</span><span class="sxs-lookup"><span data-stu-id="01abe-110">Save the policy.</span></span>
    <span data-ttu-id="01abe-111">A házirend-beállítások érvénybe léptetése akár 24 órát is igénybe vehet.</span><span class="sxs-lookup"><span data-stu-id="01abe-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="01abe-112">A webhely kizárása után törölheti a privát csatornát.</span><span class="sxs-lookup"><span data-stu-id="01abe-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="01abe-113">***Előfordulhat,*** hogy a Privát csatornát a Microsoft Teams segítségével törölheti Android-eszközén.</span><span class="sxs-lookup"><span data-stu-id="01abe-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="01abe-114">A kapcsolódó SharePoint-információk a [Nem törölhetők elemek a SharePoint Online-ban vagy a OneDrive Vállalati verzióban](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold)című témakörben olvashat.</span><span class="sxs-lookup"><span data-stu-id="01abe-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>