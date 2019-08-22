---
title: AttributeValueMustBeUnique hiba
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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527001"
---
# <a name="error-attributevaluemustbeunique"></a>Hiba: AttributeValueMustBeUnique

A leggyakoribb oka a AttributeValueMustBeUnique hiba a különböző SourceAnchor (immutableId) két objektum rendelkezik a ProxyAddresses és/vagy UserPrincipalName attribútum ugyanazt az értéket. A AttributeValueMustBeUnique hiba javításához:
  
1. Az ismétlődő proxyAddresses, userPrincipalName vagy más attribútum értéke a hibát okozó meghatározása. Az ütközés két (vagy több) objektumok részt is azonosítja. A szinkronizálás Azure AD csatlakozás egészségügyi által létrehozott jelentés segít azonosítani a két objektum.
    
2. Melyik objektum továbbra is ismétlődő értéket, és melyik objektumot nem kell azonosítani.
    
3. Távolítsa el az ismétlődő értéket az objektumot, nem kell ezt az értéket. Fontos megjegyezni, hogy kell a változtatásokat a címtárban, ha az objektum származó. Bizonyos esetekben szükség lehet az ütközés objektumok törlése.
    
4. A módosítást a helyiségben AD lehetővé teszik a Azure AD csatlakozás szinkronizálni a módosítás lehet javítani a hibát.
    

