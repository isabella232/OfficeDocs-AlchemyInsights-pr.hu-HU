---
title: 'Hiba: AttribútumÉrtékMustBeUnique'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: fa1fdb35f1af250bc98aa61c0e5111f1f1b8aac4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703176"
---
# <a name="error-attributevaluemustbeunique"></a>Hiba: AttributeValueMustBeUnique

Az AttributeValueMustBeUnique hiba leggyakoribb oka két különböző SourceAnchor (immutableId) objektum azonos értékkel rendelkezik a ProxyAddresses és/vagy a UserPrincipalName attribútumok esetében. Az AntributeValueMustBeUnique hiba javítása:
  
1. Azonosítsa a hibát okozó duplikált proxycímeket, userPrincipalName vagy más attribútumértéket. Azonosítsa azt is, hogy melyik két (vagy több) objektum érintett az ütközésben. Az Azure AD Connect Health for sync által létrehozott jelentés segítségével azonosíthatja a két objektumot.
    
2. Azonosítsa, hogy melyik objektumnak kell továbbra is rendelkeznie a duplikált értékkel, és melyik objektumnak nem szabad.
    
3. Távolítsa el a duplikált értéket abból az objektumból, amelynek NEM kellene rendelkeznie ezzel az értékkel. Ne feledje, hogy a módosítást abban a könyvtárban kell elkészíteni, ahonnan az objektum származik. Bizonyos esetekben előfordulhat, hogy törölnie kell az ütközésben lévő objektumok egyikét.
    
4. Ha a helyszíni AD-ben hajtotta végre a módosítást, hagyja, hogy az Azure AD Connect szinkronizálja a módosítást a hiba kijavításához.
    

