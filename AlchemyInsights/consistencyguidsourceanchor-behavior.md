---
title: ConsistencyGuid/sourceAnchor viselkedés
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: f0ff94a8e46f1fb4e0ac8653c51f8f651e29498b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/18/2019
ms.locfileid: "36516986"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor viselkedés

Azúrkék AD Connect (verzió 1.1.524.0 és utána) most megkönnyíti az msDS-ConsistencyGuid azonosító sourceAnchor attribútumként való használatát. Ha ezt a funkciót használja, a Azure Connect program automatikusan beállítja a szinkronizálási szabályokat:
  
- Használja a felhasználói objektumok sourceAnchor attribútumaként az msDS-ConsistencyGuid azonosítót. Az ObjectGUID objektum más objektumtípusokhoz használatos.
    
- Bármely olyan intézményi Active Directory felhasználói objektumhoz, amelynek msDS-ConsistencyGuid attribútuma nincs kitöltve, a Azure AD Connect az objectGUID értékét visszaírja az intézményi Active Directory msDS-ConsistencyGuid attribútumához. Miután az msDS-ConsistencyGuid attribútum ki van töltve, a Azure AD Connect ezután exportálja az objektumot azúrkék AD-ba.
    
 **Megjegyzés:** Miután egy intézményi Active Directory-objektumot importált a Azure AD Connect (azaz az AD Connector térbe, a metaverse értékre vetített) programba, már nem változtathatja meg a sourceAnchor értékét. Egy adott intézményi Active Directory-objektumhoz tartozó sourceAnchor azonosító megadásához konfigurálja az msDS-ConsistencyGuid attribútumot az Azure AD Connect programba történő importálás előtt. 
  
A SourceAnchor és a ConsistencyGuid azonosítóról további információt a következő címen olvashat: [Azure ad Connect: tervezési fogalmak](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

