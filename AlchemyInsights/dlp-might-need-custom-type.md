---
title: DLP esetleg szükséges egyéni típusok
ms.author: stephow
author: stephow-MSFT
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
ms.openlocfilehash: 612b6652b445914063ac825847f5698d3afc3a00
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530353"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="1a263-102">DLP esetleg szükséges egyéni típusok</span><span class="sxs-lookup"><span data-stu-id="1a263-102">DLP might need a custom type</span></span>

<span data-ttu-id="1a263-103">A veszteség megelőzése (DLP) házirend azonosítására és bizalmas adatok védelmére a szervezetben.</span><span class="sxs-lookup"><span data-stu-id="1a263-103">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="1a263-104">Bizonyos esetekben szükség lehet létrehozni saját **egyéni** bizalmas adatok védelme érdekében a szervezet adatait.</span><span class="sxs-lookup"><span data-stu-id="1a263-104">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="1a263-105">Például a szervezet kell azonosítani és alkalmazotti azonosítót vagy más néhány jellemző a org. formátumú adatok védelme Ha igen, olvassa el a következő cikkek további információt.</span><span class="sxs-lookup"><span data-stu-id="1a263-105">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="1a263-106">**Testreszabhatja a beépített érzékeny adatok típusa**</span><span class="sxs-lookup"><span data-stu-id="1a263-106">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="1a263-107">Ha a beépített érzékeny adatok típusa felel meg igényeinek, pár beállításokból állnak, testreszabhatja [a beépített érzékeny adatok típusa](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="1a263-107">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="1a263-108">Például akkor is hozzáadása vagy eltávolítása a kulcsszavak hozzáadása vagy eltávolítására dátum és cím, alátámasztó bizonyítékokat.</span><span class="sxs-lookup"><span data-stu-id="1a263-108">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="1a263-109">**Hozzon létre egy egyéni bizalmas információ típusa**</span><span class="sxs-lookup"><span data-stu-id="1a263-109">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="1a263-110">De ha azonosítására és más típusú érzékeny adatok védelmére teljesen van szüksége, [Hozzon létre egy egyéni bizalmas információ típust](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) a felhasználói felületen, a biztonsági & Megfelelési központba.</span><span class="sxs-lookup"><span data-stu-id="1a263-110">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="1a263-111">**Hozzon létre egy egyéni bizalmas információ típusa kompatibilitási központ PowerShell biztonsági &**</span><span class="sxs-lookup"><span data-stu-id="1a263-111">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="1a263-112">Végül a felhasználói felület nem rendelkeznek a szükséges beállításokat, ha hozhat [létre egy egyéni bizalmas adatok biztonsági & kompatibilitási központ PowerShell típust](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="1a263-112">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="1a263-113">XML-fájl elindításával, minden elérhető beállítás használható.</span><span class="sxs-lookup"><span data-stu-id="1a263-113">By starting with an XML file, you can use every option available.</span></span>
