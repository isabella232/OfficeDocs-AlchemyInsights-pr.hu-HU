---
title: AttributeValueMustBeUnique hiba
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7a97d1a5ff352b55833bd457e3220a56130d7e7e
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/15/2019
ms.locfileid: "28293742"
---
# <a name="error-attributevaluemustbeunique"></a>Hiba: AttributeValueMustBeUnique

A leggyakoribb oka a AttributeValueMustBeUnique hiba a különböző SourceAnchor (immutableId) két objektum rendelkezik a ProxyAddresses és/vagy UserPrincipalName attribútum ugyanazt az értéket. A AttributeValueMustBeUnique hiba javításához:
  
1. Az ismétlődő proxyAddresses, userPrincipalName vagy más attribútum értéke a hibát okozó meghatározása. Az ütközés két (vagy több) objektumok részt is azonosítja. A szinkronizálás Azure AD csatlakozás egészségügyi által létrehozott jelentés segít azonosítani a két objektum.
    
2. Melyik objektum továbbra is ismétlődő értéket, és melyik objektumot nem kell azonosítani.
    
3. Távolítsa el az ismétlődő értéket az objektumot, nem kell ezt az értéket. Fontos megjegyezni, hogy kell a változtatásokat a címtárban, ha az objektum származó. Bizonyos esetekben szükség lehet az ütközés objektumok törlése.
    
4. A módosítást a helyiségben AD lehetővé teszik a Azure AD csatlakozás szinkronizálni a módosítás lehet javítani a hibát.
    

