---
title: KonzisztenciaGuid / sourceAnchor viselkedés
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
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 8527e7c2404742a999041f85ed12d78c48cc0d8c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705735"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>KonzisztenciaGuid / sourceAnchor viselkedés

Az Azure AD Connect (1.1.524.0-s és újabb verzió) mostantól megkönnyíti az msDS-ConsistencyGuid sourceAnchor attribútumként való használatát. A funkció használatakor az Azure AD Connect automatikusan konfigurálja a szinkronizálási szabályokat a következőkre:
  
- Használja az msDS-ConsistencyGuid-ot a felhasználói objektumok sourceAnchor attribútumaként. Az ObjectGUID más objektumtípusokhoz is használható.
    
- Minden olyan helyszíni AD-felhasználó objektum, amelynek msDS-consistencyGuid attribútum nincs feltöltve, az Azure AD Connect írja az objectGUID értékét vissza az msDS-consistencyGuid attribútum a helyszíni Active Directoryban. Az msDS-ConsistencyGuid attribútum feltöltése után az Azure AD Connect exportálja az objektumot az Azure AD-be.
    
 **Megjegyzés:** Miután egy helyszíni AD-objektum ot importált az Azure AD Connect (azaz az AD-összekötő térbe importálva és a Metaverzumba vetítve), többé nem módosíthatja a sourceAnchor értékét. Egy adott helyszíni AD-objektum sourceAnchor értékének megadásához konfigurálja az msDS-ConsistencyGuid attribútumot az Azure AD Connectbe történő importálás előtt. 
  
A SourceAnchor és a ConsistencyGuid használatával kapcsolatos további információkért tekintse meg a következő t: [Azure AD Connect: Tervezési fogalmak](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

