---
title: Error AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 35eb88624a5535e136ac1d01faf8e905bf00eb45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813762"
---
# <a name="error-attributevaluemustbeunique"></a>Hiba: AttributeValueMustBeUnique

Az AttributeValueMustBeUnique hiba leggyakoribb oka két különböző SourceAnchor (immutableId) attribútummal azonos értékű a ProxyAddresses és/vagy a UserPrincipalName attribútumban. Az AttributeValueMustBeUnique hiba kijavítani:
  
1. Azonosítsa a hibát okozó duplikált proxyAddresses, userPrincipalName vagy más attribútumértéket. Azonosítsa azt is, hogy melyik két (vagy több) objektum érintett az ütközésben. Az Azure AD Connect Health for Sync által létrehozott jelentés segíthet azonosítani a két objektumot.
    
2. Azonosítsa, hogy melyik objektumnak legyen a duplikált értéke, és melyik objektumnak ne.
    
3. Távolítsa el a duplikált értéket az objektumból, amely nem lehet ilyen értékkel. Ne feledje, hogy a módosításnak abban a címtárban kell lennie, amelyből az objektum származik. Bizonyos esetekben előfordulhat, hogy törölnie kell az ütközésben lévő objektumok valamelyikét.
    
4. Ha a változtatást a helyszíni AD-ban tette, hagyja, hogy az Azure AD Connect szinkronizálja a változást, hogy kijavítsa a hibát.
    

