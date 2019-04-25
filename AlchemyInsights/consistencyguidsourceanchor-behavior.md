---
title: ConsistencyGuid / sourceAnchor viselkedés
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
ms.openlocfilehash: cb1b50792b07a1b3b69607bf2f6824141a15922f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/23/2019
ms.locfileid: "32408110"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor viselkedés

Azure AD csatlakozás (1.1.524.0 verzió, és utána) most lehetővé teszi az msDS-ConsistencyGuid sourceAnchor attribútum használatát. Ez a funkció használatakor Azure AD csatlakozás automatikusan beállítja a szinkronizálási szabályok:
  
- A sourceAnchor attribútum a felhasználói objektum msDS-ConsistencyGuid használják. ObjectGUID más objektumtípusok esetében használatos.
    
- Bármely adott helyszíni AD felhasználói objektum, amelynek msDS-ConsistencyGuid attribútumot nem lakott, Azure AD csatlakozás írások az objectGUID értéket vissza a helyszíni Active Directory msDS-ConsistencyGuid attribútumot. Miután az msDS-ConsistencyGuid attribútumot nem üres, Azure AD csatlakozás majd exportálja az objektum Azure AD.
    
 **Megjegyzés:** Egyszer helyszíni AD objektum Azure AD csatlakozás (azaz, importálja a összekötő AD helyet, és a Metaverse vetített) importálja, az sourceAnchor értékét már nem módosíthatja. Adhatja meg a sourceAnchor értékét egy adott helyszíni AD az objektum, az msDS-ConsistencyGuid attribútumot konfigurálása előtt Azure AD csatlakozás lesz importálva. 
  
SourceAnchor és ConsistencyGuid további információt talál a következő: [Azure AD csatlakozás: tervezési koncepciók](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

