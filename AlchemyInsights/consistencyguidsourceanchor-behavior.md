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
ms.openlocfilehash: 9b5765ff3c59b1312bead41a45a53478a96260df0567f006ab93c3ccfaf4be64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044342"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>KonzisztenciaGuid/sourceAnchor behavior

Az Azure AD Csatlakozás (1.1.524.0-s és újabb verzió) mostantól megkönnyíti az msDS-ConsistencyGuid forrásAnchor attribútumként való használatát. A funkció használata során az Azure AD Csatlakozás automatikusan konfigurálja a szinkronizálási szabályokat a következőre:
  
- A user objektumok sourceAnchor attribútumaként használja az msDS-ConsistencyGuid attribútumot. Az ObjectGUID más objektumtípusokhoz használatos.
    
- Minden olyan helyszíni AD User objektum esetében, amelynek msDS-ConsistencyGuid attribútuma nincs feltöltve, az Azure AD Csatlakozás visszaírja az objectGUID értékét az msDS-ConsistencyGuid attribútumba a helyszíni Active Directoryban. Az msDS-ConsistencyGuid attribútum feltöltése után az Azure AD Csatlakozás exportálja az objektumot az Azure AD-be.
    
 **Megjegyzés:** Miután egy helyszíni AD-objektumot importált az Azure AD Csatlakozás-be (amely az AD-összekötő térbe importálása és a Metaverzába való kivetítve történik), a forrásAnchor érték többé nem változtatható meg. A sourceAnchor érték megadásához egy adott helyszíni AD-objektumhoz konfigurálja az msDS-ConsistencyGuid attribútumot, mielőtt az importálva lenne az Azure AD-Csatlakozás. 
  
A SourceAnchor és a ConsistencyGuid szolgáltatásról további információt az [Azure AD Csatlakozás: Tervezési fogalmak](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

