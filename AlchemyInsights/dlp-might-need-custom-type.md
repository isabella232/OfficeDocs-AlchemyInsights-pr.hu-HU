---
title: A DLP-nek szüksége lehet egy egyéni típusra
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
ms.openlocfilehash: 872fca326065ada002300061c951620b3d9a8d0e
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052903"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="91017-102">A DLP-nek szüksége lehet egy egyéni típusra</span><span class="sxs-lookup"><span data-stu-id="91017-102">DLP might need a custom type</span></span>

<span data-ttu-id="91017-103">Az adatvesztésmegelőzési (DLP) házirend segítségével azonosíthatja és megvédheti a bizalmas adatokat a szervezeten belül.</span><span class="sxs-lookup"><span data-stu-id="91017-103">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="91017-104">Egyes esetekben szükség lehet arra, hogy a szervezeti adatok védelme érdekében **Egyéni** , bizalmas adattípusra legyen szüksége.</span><span class="sxs-lookup"><span data-stu-id="91017-104">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="91017-105">Előfordulhat például, hogy a szervezetnek azonosítania kell és meg kell védenie az alkalmazotti azonosítókat vagy más adatokat a szervezet bizonyos formátumában. Ha igen, további információért olvassa el az alábbi cikkeket.</span><span class="sxs-lookup"><span data-stu-id="91017-105">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="91017-106">**Beépített érzékeny adattípus testreszabása**</span><span class="sxs-lookup"><span data-stu-id="91017-106">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="91017-107">Ha egy beépített érzékeny adattípus csak néhány csíp, akkor tudja, [testre szabhatja a beépített érzékeny információ típusát](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="91017-107">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="91017-108">Hozzáadhat vagy eltávolíthat kulcsszavakat, vagy hozzáadhat vagy eltávolíthat olyan alátámasztó bizonyítékokat, mint például dátum vagy cím.</span><span class="sxs-lookup"><span data-stu-id="91017-108">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="91017-109">**Egyéni szenzitív adattípus létrehozása**</span><span class="sxs-lookup"><span data-stu-id="91017-109">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="91017-110">Ha azonban egy másik típusú érzékeny információt is azonosítani és védeni kell, akkor [létrehozhat egy egyedi, érzékeny adattípust](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) a biztonsági & megfelelőségi központ felhasználói felületén.</span><span class="sxs-lookup"><span data-stu-id="91017-110">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="91017-111">**Egyéni érzékeny adattípus létrehozása a biztonsági & megfelelőségi központ PowerShell eszközzel**</span><span class="sxs-lookup"><span data-stu-id="91017-111">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="91017-112">Végül, ha a felhasználói felület nem biztosítja az összes szükséges lehetőséget, létrehozhat [egy egyéni érzékeny adattípustípust is a biztonsági & a megfelelőségi központ PowerShell parancshéjban](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="91017-112">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="91017-113">Az XML-fájllal kezdve minden rendelkezésre álló opciót igénybe lehet használni.</span><span class="sxs-lookup"><span data-stu-id="91017-113">By starting with an XML file, you can use every option available.</span></span>
