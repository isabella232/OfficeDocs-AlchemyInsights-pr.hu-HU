---
title: A DLP nem a várt módon működik
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932624"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="5faef-102">A DLP nem a várt módon működik</span><span class="sxs-lookup"><span data-stu-id="5faef-102">DLP not working as expected</span></span>

<span data-ttu-id="5faef-103">**Fontos:** Sok SharePoint Online- és OneDrive-ügyfél üzleti szempontból kritikus fontosságú alkalmazásokat futtat a háttérben futó szolgáltatással szemben.</span><span class="sxs-lookup"><span data-stu-id="5faef-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="5faef-104">Ezek közé tartozik a tartalomáttelepítés, az adatveszteség-megelőzés (DLP) és a biztonsági mentési megoldások.</span><span class="sxs-lookup"><span data-stu-id="5faef-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="5faef-105">Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive-szolgáltatások magas rendelkezésre állásúak és megbízhatóak maradjanak a távoli munkahelyi helyzetekben minden eddiginél jobban függő felhasználók számára.</span><span class="sxs-lookup"><span data-stu-id="5faef-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="5faef-106">Ennek a célkitűzésnek a támogatása érdekében szigorúbb szabályozási korlátokat vezettünk be a háttéralkalmazásokra (áttelepítés, DLP és biztonsági mentési megoldások) a hétköznapokon.</span><span class="sxs-lookup"><span data-stu-id="5faef-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="5faef-107">Meg kell várni, hogy ezek az alkalmazások elérése nagyon korlátozott átviteli ezekben az időkben.</span><span class="sxs-lookup"><span data-stu-id="5faef-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="5faef-108">Azonban a régió esti és hétvégi óráiban a szolgáltatás készen áll arra, hogy jelentősen nagyobb mennyiségű kérést dolgozzon fel a háttéralkalmazásokból.</span><span class="sxs-lookup"><span data-stu-id="5faef-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

 <span data-ttu-id="5faef-109">**A DLP beállítása**</span><span class="sxs-lookup"><span data-stu-id="5faef-109">**Setting up DLP**</span></span>

<span data-ttu-id="5faef-110">Problémái vannak az **adatvesztés-megelőzéssel (DLP)** az Office 365-ben, hogy nem a várt módon működnek?</span><span class="sxs-lookup"><span data-stu-id="5faef-110">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="5faef-111">Ha igen, győződjön meg arról, hogy a **DLP-házirend** megfelelően van beállítva, és hogy az adatok tartalmazzák, amit a **DLP-házirend** keres, amikor kiértékelik.</span><span class="sxs-lookup"><span data-stu-id="5faef-111">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="5faef-112">A DLP-házirendek lehetővé teszik a szervezeten belüli bizalmas adatok azonosítását és védelmét.</span><span class="sxs-lookup"><span data-stu-id="5faef-112">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="5faef-113">A DLP-házirendek beállításához használja az [itt](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)található információkat.</span><span class="sxs-lookup"><span data-stu-id="5faef-113">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="5faef-114">**Mit keresnek a DLP-házirendek?**</span><span class="sxs-lookup"><span data-stu-id="5faef-114">**What DLP policies look for**</span></span>
  
<span data-ttu-id="5faef-115">Ha az Office 365 Biztonsági és megfelelőségi központban **a beépített bizalmas információtípusokat** használja, a DLP-házirendek az ilyen bizalmas típusok észlelésekor konkrét mintákat és elemeket keresnek.</span><span class="sxs-lookup"><span data-stu-id="5faef-115">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="5faef-116">**Beépített bizalmas információtípusok**</span><span class="sxs-lookup"><span data-stu-id="5faef-116">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="5faef-117">A beépített bizalmas típusokról és a DLP-házirend ről a Bizalmas típus észlelésekor a következő témakörben talál tájékoztatást: [A bizalmas információtípusok keresetttémaköre.](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="5faef-117">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="5faef-118">**Egyéni bizalmas információtípusok**</span><span class="sxs-lookup"><span data-stu-id="5faef-118">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="5faef-119">Ha egyéni bizalmas információtípusokat próbál létrehozni, az alábbi cikkben megtudhatja, hogyan hozhat létre egyéni bizalmas [szöveget: Egyéni bizalmas információtípus létrehozása](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="5faef-119">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="5faef-120">**DLP-házirend tesztelése**</span><span class="sxs-lookup"><span data-stu-id="5faef-120">**Test a DLP policy**</span></span>

<span data-ttu-id="5faef-121">Ha az adatokat beépített vagy egyéni bizalmas adatoktípussal szeretné tesztelni, használja a **Teszttípus** beállítást a **Besorolások** > **bizalmas információtípusai**csoportban.</span><span class="sxs-lookup"><span data-stu-id="5faef-121">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="5faef-122">További információt az [Egyéni bizalmas információtípusok tesztelése](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center)című témakörben talál.</span><span class="sxs-lookup"><span data-stu-id="5faef-122">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="5faef-123">**Jelentések**</span><span class="sxs-lookup"><span data-stu-id="5faef-123">**Reports**</span></span>
  
- <span data-ttu-id="5faef-124">Bizalmas adatok betekintést nyerhet a [DLP-jelentések segítségével.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="5faef-124">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="5faef-125">Az esemény konkrét részleteinek megtekintése [incidensjelentéssel.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)</span><span class="sxs-lookup"><span data-stu-id="5faef-125">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
