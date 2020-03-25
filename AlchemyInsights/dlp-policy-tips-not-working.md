---
title: A DLP házirendtippjei nem működnek
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932588"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="136df-102">DLP-házirend tippjével kapcsolatos problémák</span><span class="sxs-lookup"><span data-stu-id="136df-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="136df-103">**Fontos:** Sok SharePoint Online- és OneDrive-ügyfél üzleti szempontból kritikus fontosságú alkalmazásokat futtat a háttérben futó szolgáltatással szemben.</span><span class="sxs-lookup"><span data-stu-id="136df-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="136df-104">Ezek közé tartozik a tartalomáttelepítés, az adatveszteség-megelőzés (DLP) és a biztonsági mentési megoldások.</span><span class="sxs-lookup"><span data-stu-id="136df-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="136df-105">Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive-szolgáltatások magas rendelkezésre állásúak és megbízhatóak maradjanak a távoli munkahelyi helyzetekben minden eddiginél jobban függő felhasználók számára.</span><span class="sxs-lookup"><span data-stu-id="136df-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="136df-106">Ennek a célkitűzésnek a támogatása érdekében szigorúbb szabályozási korlátokat vezettünk be a háttéralkalmazásokra (áttelepítés, DLP és biztonsági mentési megoldások) a hétköznapokon.</span><span class="sxs-lookup"><span data-stu-id="136df-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="136df-107">Meg kell várni, hogy ezek az alkalmazások elérése nagyon korlátozott átviteli ezekben az időkben.</span><span class="sxs-lookup"><span data-stu-id="136df-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="136df-108">Azonban a régió esti és hétvégi óráiban a szolgáltatás készen áll arra, hogy jelentősen nagyobb mennyiségű kérést dolgozzon fel a háttéralkalmazásokból.</span><span class="sxs-lookup"><span data-stu-id="136df-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="136df-109">**DLP-házirendtippek**</span><span class="sxs-lookup"><span data-stu-id="136df-109">**DLP policy tips**</span></span>

<span data-ttu-id="136df-110">A **DLP-házirendek**használatakor a felhasználók értesítést kaphatnak a házirendek megsértéséről a **házirend-tippekkel.**</span><span class="sxs-lookup"><span data-stu-id="136df-110">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="136df-111">A rendszergazdák beállíthatják, hogy a házirend-tippek a DLP-házirend tesztelése közben, vagy ha a házirend teljes kényszerítési módban van.</span><span class="sxs-lookup"><span data-stu-id="136df-111">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="136df-112">Ha a DLP-házirenddel kapcsolatos házirendtippeket teljes kényszerítési módban szeretné konfigurálni a Biztonsági és megfelelőségi központban, tegye a következőket:</span><span class="sxs-lookup"><span data-stu-id="136df-112">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="136df-113">Győződjön meg arról, hogy a DLP-szabályban **engedélyezve** vannak a házirendtippek az [itt](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)leírt lépésekkel.</span><span class="sxs-lookup"><span data-stu-id="136df-113">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="136df-114">Győződjön meg arról, hogy a **tartalom megfelel** a [cikkben](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)ismertetett szabály aktiválásához **szükséges módon.**</span><span class="sxs-lookup"><span data-stu-id="136df-114">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="136df-115">A házirendtippek az OWA-ban és az Outlookban is megjelennek.</span><span class="sxs-lookup"><span data-stu-id="136df-115">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="136df-116">Az Outlook **2013-as vagy újabb**verzióinak használatakor azonban a házirendtippek csak bizonyos körülmények között jelennek meg.</span><span class="sxs-lookup"><span data-stu-id="136df-116">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="136df-117">Ezek a feltételek itt találhatók: [Az Outlook 2013-as vagy újabb verzióinak támogatott feltételei a házirendtippek megjelenítéséhez](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span><span class="sxs-lookup"><span data-stu-id="136df-117">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span></span>

<span data-ttu-id="136df-118">A DLP-házirendekkel kapcsolatos tippekről a Következő témakörben [olvashat: Házirendtippek megjelenítése a DLP-házirendekhez](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="136df-118">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span></span>
  