---
title: ConsistencyGuid/sourceAnchor viselkedése
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
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: adac469328485696d1ee1532aa3d6828af0642eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756285"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor viselkedése

Azure AD Connect (1.1.524.0-es verzió) most már megkönnyíti az msDS-ConsistencyGuid as sourceAnchor attribútum használatát. A funkció használatakor az Azure AD Connect automatikusan beállítja a szinkronizálási szabályokat az alábbiak szerint:
  
- Használja az msDS-ConsistencyGuid, mint a felhasználói objektumok sourceAnchor attribútumát. A ObjectGUID más objektumtípusok számára van használatban.
    
- Ha a helyszíni AD User objektumnak nincs kitöltve az msDS-ConsistencyGuid attribútuma, akkor az Azure AD Connect az objectGUID értékét visszaállítja a helyszíni Active Directory-beli msDS-ConsistencyGuid attribútumra. Az msDS-ConsistencyGuid attribútum feltöltése után az Azure AD Connect ezt követően exportálja az objektumot az Azure AD-ra.
    
 **Megjegyzés:** Ha a helyszíni AD-objektumot importálta az Azure AD Connectbe (azaz az AD Connector-területre importálja, és a metaverse-ba tervezi), már nem módosíthatja a sourceAnchor értékét. Ha a helyszíni AD objektum sourceAnchor értékét szeretné megadni, akkor állítsa be az msDS-ConsistencyGuid attribútumot, mielőtt az Azure AD Connect programba importálja őket. 
  
A SourceAnchor és a ConsistencyGuid további információt a következő témakörben találhat: [Azure ad Connect: tervezési fogalmak](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

