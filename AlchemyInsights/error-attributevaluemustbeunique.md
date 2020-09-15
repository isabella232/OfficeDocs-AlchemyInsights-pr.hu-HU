---
title: AttributeValueMustBeUnique hiba
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 4627a7ae34b0dd9f16538ef75ac8792672dcc056
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709153"
---
# <a name="error-attributevaluemustbeunique"></a>Hiba: AttributeValueMustBeUnique

A AttributeValueMustBeUnique hibájának leggyakoribb oka két különböző SourceAnchor (immutableId) rendelkező objektum, amely a ProxyAddresses és/vagy a UserPrincipalName attribútummal azonos értékű. A AttributeValueMustBeUnique hibájának kijavítása:
  
1. Azonosítsa a duplikált proxyAddresses, a userPrincipalName vagy más, a hibát okozó attribútum értékét. Azt is megadhatja, hogy mely két (vagy több) objektum vesz részt az ütközésben. Az Azure AD Connect Health for Sync által generált jelentés segítséget nyújt a két objektum felismerésében.
    
2. Annak meghatározása, hogy melyik objektumnak legyen a duplikált értéke, és melyik objektumnak kell maradnia.
    
3. Távolítsa el a duplikált értéket az objektumról, amelynek nem kell ezt az értéket tartalmaznia. Fontos tudni, hogy a módosítást abban a könyvtárban végezze el, ahol az objektum származik. Bizonyos esetekben előfordulhat, hogy törölnie kell az ütközést okozó objektumok egyikét.
    
4. Ha módosította a helyszíni HIRDETÉSt, engedje meg, hogy az Azure AD Connect szinkronizálja a hiba módosítását a kijavításhoz.
    

