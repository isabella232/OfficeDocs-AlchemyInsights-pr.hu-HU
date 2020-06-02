---
title: Előfordulhat, hogy a DLP-nek egyéni típusra van szüksége
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1ec8959a479f1a8f7bfcffb55f440e8c4ab435fb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507516"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="0c6be-102">Előfordulhat, hogy a DLP-nek egyéni típusra van szüksége</span><span class="sxs-lookup"><span data-stu-id="0c6be-102">DLP might need a custom type</span></span>

<span data-ttu-id="0c6be-103">**Fontos**: Ezekben a példátlan időkben lépéseket teszünk annak biztosítására, hogy a SharePoint Online és a OneDrive szolgáltatások továbbra is mindig hozzáférhetők legyenek – További információt a [SharePoint Online Ideiglenes funkciómódosítások](https://aka.ms/ODSPAdjustments) oldalon olvashat.</span><span class="sxs-lookup"><span data-stu-id="0c6be-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="0c6be-104">**A DLP-hez egyéni információtípusra lehet szükség**</span><span class="sxs-lookup"><span data-stu-id="0c6be-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="0c6be-105">Az adatvesztés-megelőzési (DLP) házirenddel azonosíthatja és megvédheti a szervezeten belüli bizalmas adatokat.</span><span class="sxs-lookup"><span data-stu-id="0c6be-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="0c6be-106">Bizonyos esetekben előfordulhat, hogy létre kell hoznia saját **egyéni** bizalmas információtípusát a szervezet adatainak védelme érdekében.</span><span class="sxs-lookup"><span data-stu-id="0c6be-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="0c6be-107">Előfordulhat például, hogy a szervezetnek azonosítania és védenie kell az alkalmazottazonosítókat vagy más adatokat a szervezetre jellemző formátumban. Ha igen, további információt az alábbi cikkekben talál.</span><span class="sxs-lookup"><span data-stu-id="0c6be-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="0c6be-108">**Beépített bizalmas információtípus testreszabása**</span><span class="sxs-lookup"><span data-stu-id="0c6be-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="0c6be-109">Ha egy beépített bizalmas információtípus néhány csípéssel megfelel az igényeinek, [testreszabhatja a beépített bizalmas információtípust.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type)</span><span class="sxs-lookup"><span data-stu-id="0c6be-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="0c6be-110">Hozzáadhat vagy eltávolíthat például kulcsszavakat, illetve hozzáadhat vagy eltávolíthat alátámasztó bizonyítékokat, például dátumot vagy címet.</span><span class="sxs-lookup"><span data-stu-id="0c6be-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="0c6be-111">**Egyéni bizalmas információtípus létrehozása**</span><span class="sxs-lookup"><span data-stu-id="0c6be-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="0c6be-112">Ha azonban egy másik típusú bizalmas információt kell azonosítania és védenie, [létrehozhat egy egyéni bizalmas információtípust](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) a Biztonsági & megfelelőségi központ felhasználói felületén.</span><span class="sxs-lookup"><span data-stu-id="0c6be-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="0c6be-113">**Egyéni bizalmas információtípus létrehozása a Security & Compliance Center PowerShell ben**</span><span class="sxs-lookup"><span data-stu-id="0c6be-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="0c6be-114">Végül, ha a felhasználói felület nem biztosítja az összes szükséges beállítást, [létrehozhat egy egyéni bizalmas információtípust a Security & Compliance Center PowerShell ben.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="0c6be-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="0c6be-115">Az XML-fájllal kezdve minden elérhető lehetőséget használhat.</span><span class="sxs-lookup"><span data-stu-id="0c6be-115">By starting with an XML file, you can use every option available.</span></span>
