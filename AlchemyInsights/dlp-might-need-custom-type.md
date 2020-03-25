---
title: Előfordulhat, hogy a DLP-nek egyéni típusra van szüksége
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932660"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="8da92-102">Előfordulhat, hogy a DLP-nek egyéni típusra van szüksége</span><span class="sxs-lookup"><span data-stu-id="8da92-102">DLP might need a custom type</span></span>

<span data-ttu-id="8da92-103">**Fontos:** Sok SharePoint Online- és OneDrive-ügyfél üzleti szempontból kritikus fontosságú alkalmazásokat futtat a háttérben futó szolgáltatással szemben.</span><span class="sxs-lookup"><span data-stu-id="8da92-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="8da92-104">Ezek közé tartozik a tartalomáttelepítés, az adatveszteség-megelőzés (DLP) és a biztonsági mentési megoldások.</span><span class="sxs-lookup"><span data-stu-id="8da92-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="8da92-105">Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive-szolgáltatások magas rendelkezésre állásúak és megbízhatóak maradjanak a távoli munkahelyi helyzetekben minden eddiginél jobban függő felhasználók számára.</span><span class="sxs-lookup"><span data-stu-id="8da92-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="8da92-106">Ennek a célkitűzésnek a támogatása érdekében szigorúbb szabályozási korlátokat vezettünk be a háttéralkalmazásokra (áttelepítés, DLP és biztonsági mentési megoldások) a hétköznapokon.</span><span class="sxs-lookup"><span data-stu-id="8da92-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="8da92-107">Meg kell várni, hogy ezek az alkalmazások elérése nagyon korlátozott átviteli ezekben az időkben.</span><span class="sxs-lookup"><span data-stu-id="8da92-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="8da92-108">Azonban a régió esti és hétvégi óráiban a szolgáltatás készen áll arra, hogy jelentősen nagyobb mennyiségű kérést dolgozzon fel a háttéralkalmazásokból.</span><span class="sxs-lookup"><span data-stu-id="8da92-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="8da92-109">**A DLP-hez egyéni információtípusra lehet szükség**</span><span class="sxs-lookup"><span data-stu-id="8da92-109">**DLP may require a custom information type**</span></span>

<span data-ttu-id="8da92-110">Az adatvesztés-megelőzési (DLP) házirenddel azonosíthatja és megvédheti a szervezeten belüli bizalmas adatokat.</span><span class="sxs-lookup"><span data-stu-id="8da92-110">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="8da92-111">Bizonyos esetekben előfordulhat, hogy létre kell hoznia saját **egyéni** bizalmas információtípusát a szervezet adatainak védelme érdekében.</span><span class="sxs-lookup"><span data-stu-id="8da92-111">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="8da92-112">Előfordulhat például, hogy a szervezetnek azonosítania és védenie kell az alkalmazottazonosítókat vagy más adatokat a szervezetre jellemző formátumban. Ha igen, további információt az alábbi cikkekben talál.</span><span class="sxs-lookup"><span data-stu-id="8da92-112">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="8da92-113">**Beépített bizalmas információtípus testreszabása**</span><span class="sxs-lookup"><span data-stu-id="8da92-113">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="8da92-114">Ha egy beépített bizalmas információtípus néhány csípéssel megfelel az igényeinek, [testreszabhatja a beépített bizalmas információtípust.](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="8da92-114">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="8da92-115">Hozzáadhat vagy eltávolíthat például kulcsszavakat, illetve hozzáadhat vagy eltávolíthat alátámasztó bizonyítékokat, például dátumot vagy címet.</span><span class="sxs-lookup"><span data-stu-id="8da92-115">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="8da92-116">**Egyéni bizalmas információtípus létrehozása**</span><span class="sxs-lookup"><span data-stu-id="8da92-116">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="8da92-117">Ha azonban egy másik típusú bizalmas információt kell azonosítania és védenie, [létrehozhat egy egyéni bizalmas információtípust](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) a Biztonsági & megfelelőségi központ felhasználói felületén.</span><span class="sxs-lookup"><span data-stu-id="8da92-117">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="8da92-118">**Egyéni bizalmas információtípus létrehozása a Security & Compliance Center PowerShell ben**</span><span class="sxs-lookup"><span data-stu-id="8da92-118">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="8da92-119">Végül, ha a felhasználói felület nem biztosítja az összes szükséges beállítást, [létrehozhat egy egyéni bizalmas információtípust a Security & Compliance Center PowerShell ben.](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="8da92-119">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="8da92-120">Az XML-fájllal kezdve minden elérhető lehetőséget használhat.</span><span class="sxs-lookup"><span data-stu-id="8da92-120">By starting with an XML file, you can use every option available.</span></span>
