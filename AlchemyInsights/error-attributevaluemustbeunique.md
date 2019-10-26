---
title: Hiba AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 5ac56fa78c66cf3b246bc0cc01f040e27310d629
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/25/2019
ms.locfileid: "36527001"
---
# <a name="error-attributevaluemustbeunique"></a>Hiba: AttributeValueMustBeUnique

Az AttributeValueMustBeUnique hiba leggyakoribb oka, hogy két objektum különböző SourceAnchor (immutableId), értéke megegyezik a ProxyAddresses és/vagy UserPrincipalName attribútumokkal. -Hoz erősít a AttributeValueMustBeUnique hiba:
  
1. Azonosságot megállapít a duplázott proxyAddresses, userPrincipalName vagy más tulajdonság érték amit ' okozás a hiba. Azt is azonosítsa, hogy mely két (vagy több) objektum vesz részt a konfliktusban. Ez a jelentés segít a két objektum azonosításában, amennyiben az Azure AD Connect Health szinkronizálta a szinkronizálást.
    
2. Azonosítsa, hogy melyik objektumnak kell folytatnia a duplikált értéket, és hogy melyik objektumnak kell lennie.
    
3. Távolítsa el a duplikált értéket az objektumból, amelynek nem kellett volna ezt az értéket tartalmaznia. Ne feledje, hogy meg kell tennie a változást a könyvtárban, ahol az objektum származik. Bizonyos esetekben előfordulhat, hogy törölnie kell egy ütköző objektumot.
    
4. Ha a helyszíni Active Directory-ban módosítja a változást, akkor a Azure AD Connect segítségével a hibát kijavítottuk.
    

