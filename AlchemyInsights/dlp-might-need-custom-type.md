---
title: A DLP szükség lehet egyéni típusra
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712186"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="39396-102">A DLP szükség lehet egyéni típusra</span><span class="sxs-lookup"><span data-stu-id="39396-102">DLP might need a custom type</span></span>

<span data-ttu-id="39396-103">**Fontos**: Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatások továbbra is mindig hozzáférhetők legyenek – További információt a [SharePoint Online Ideiglenes funkciómódosítások](https://aka.ms/ODSPAdjustments) oldalon olvashat.</span><span class="sxs-lookup"><span data-stu-id="39396-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="39396-104">**A DLP egyéni adattípust igényelhet**</span><span class="sxs-lookup"><span data-stu-id="39396-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="39396-105">Az adatvesztés-megakadályozási házirend segítségével bizalmas adatokat azonosíthat és védheti meg a szervezetében.</span><span class="sxs-lookup"><span data-stu-id="39396-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="39396-106">Bizonyos esetekben előfordulhat, hogy saját **Egyéni** bizalmas adattípust kell létrehoznia a szervezeti adatok védelme érdekében.</span><span class="sxs-lookup"><span data-stu-id="39396-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="39396-107">Előfordulhat például, hogy a szervezete az alkalmazottak azonosítóit vagy más adatait az Ön szervezetéhez tartozó bizonyos formátumban kell megállapítania és védenie. Ha igen, további információért olvassa el az alábbi cikkeket.</span><span class="sxs-lookup"><span data-stu-id="39396-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="39396-108">**Beépített bizalmas adattípus testreszabása**</span><span class="sxs-lookup"><span data-stu-id="39396-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="39396-109">Ha egy beépített bizalmas adattípus csak néhány csípéssel felel meg az igényeinek, [testre szabhatja a beépített bizalmas adattípust](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="39396-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="39396-110">Hozzáadhat vagy eltávolíthat például kulcsszavakat, illetve alátámasztó bizonyítékokat, például dátumot vagy címeket adhat hozzá vagy távolíthat el.</span><span class="sxs-lookup"><span data-stu-id="39396-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="39396-111">**Egyéni bizalmas adattípus létrehozása**</span><span class="sxs-lookup"><span data-stu-id="39396-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="39396-112">Ha azonban egy eltérő típusú bizalmas információt is el kell végeznie, akkor [Egyéni bizalmas adattípust hozhat létre](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) a biztonsági & megfelelőségi központ felhasználói felületén.</span><span class="sxs-lookup"><span data-stu-id="39396-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="39396-113">**Egyéni bizalmas adattípus létrehozása a biztonsági & megfelelőségi központ PowerShellben**</span><span class="sxs-lookup"><span data-stu-id="39396-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="39396-114">Végül ha a felhasználói felület nem adja meg a szükséges beállításokat, [létrehozhat egy egyéni bizalmas adattípust a biztonsági & megfelelőségi központ PowerShellben](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="39396-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="39396-115">Az XML-fájllal kezdve minden elérhető lehetőséget használhat.</span><span class="sxs-lookup"><span data-stu-id="39396-115">By starting with an XML file, you can use every option available.</span></span>
