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
ms.openlocfilehash: 37d6764d19d9cfbb0899a5ab85a4b1530896568adc364122075b7d6f2a32970a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54002122"
---
# <a name="error-attributevaluemustbeunique"></a>Hiba: AttributeValueMustBeUnique

Az AttributeValueMustBeUnique hiba leggyakoribb oka két különböző SourceAnchor (immutableId) attribútummal azonos értékű a ProxyAddresses és/vagy a UserPrincipalName attribútumban. Az AttributeValueMustBeUnique hiba kijavítani:
  
1. Azonosítsa a hibát okozó duplikált proxyAddresses, userPrincipalName vagy más attribútumértéket. Azonosítsa azt is, hogy melyik két (vagy több) objektum érintett az ütközésben. Az Azure AD Csatlakozás Health for Sync által létrehozott jelentés segíthet azonosítani a két objektumot.
    
2. Azonosítsa, hogy melyik objektumnak legyen a duplikált értéke, és melyik objektumnak ne.
    
3. Távolítsa el a duplikált értéket az objektumból, amely nem lehet ilyen értékkel. Ne feledje, hogy a módosításnak abban a címtárban kell lennie, amelyből az objektum származik. Bizonyos esetekben előfordulhat, hogy törölnie kell az ütközésben lévő objektumok valamelyikét.
    
4. Ha a változtatást a helyszíni AD-ban tette meg, hagyja, hogy az Azure AD Csatlakozás szinkronizálja a változást a hiba kijavítása miatt.
    

