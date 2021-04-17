---
title: KonzisztenciaGuid/sourceAnchor behavior
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
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816994"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>KonzisztenciaGuid/sourceAnchor behavior

Az Azure AD Connect (1.1.524.0-s és újabb verzió) mostantól megkönnyíti az msDS-ConsistencyGuid használatát sourceAnchor attribútumként. A funkció használata esetén az Azure AD Connect automatikusan konfigurálja a szinkronizálási szabályokat a következő módon:
  
- A user objektumok sourceAnchor attribútumaként használja az msDS-ConsistencyGuid attribútumot. Az ObjectGUID más objektumtípusokhoz használatos.
    
- Minden olyan helyszíni AD User objektum esetében, amelynek msDS-ConsistencyGuid attribútuma nincs feltöltve, az Azure AD Connect visszaírja az objektumGUID értékét az msDS-ConsistencyGuid attribútumba a helyszíni Active Directoryban. Az msDS-ConsistencyGuid attribútum feltöltése után az Azure AD Connect ezután exportálja az objektumot az Azure AD szolgáltatásba.
    
 **Megjegyzés:** Miután egy helyszíni AD-objektumot importált az Azure AD Connect szolgáltatásba (amely az AD Connector Szóközbe importálva, majd a Metaverzába kivetítve történt), már nem módosíthatja a forrásAnchor értékét. A sourceAnchor érték megadásához egy adott helyszíni AD-objektumhoz konfigurálja az msDS-ConsistencyGuid attribútumot az Azure AD Connectbe való importálás előtt. 
  
További információ a SourceAnchor és a ConsistencyGuid szolgáltatásról: [Azure AD Connect:](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts) Tervezési fogalmak
  

