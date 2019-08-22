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
ms.openlocfilehash: f0ff94a8e46f1fb4e0ac8653c51f8f651e29498b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516986"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor viselkedés

Azure AD csatlakozás (1.1.524.0 verzió, és utána) most lehetővé teszi az msDS-ConsistencyGuid sourceAnchor attribútum használatát. Ez a funkció használatakor Azure AD csatlakozás automatikusan beállítja a szinkronizálási szabályok:
  
- A sourceAnchor attribútum a felhasználói objektum msDS-ConsistencyGuid használják. ObjectGUID más objektumtípusok esetében használatos.
    
- Bármely adott helyszíni AD felhasználói objektum, amelynek msDS-ConsistencyGuid attribútumot nem lakott, Azure AD csatlakozás írások az objectGUID értéket vissza a helyszíni Active Directory msDS-ConsistencyGuid attribútumot. Miután az msDS-ConsistencyGuid attribútumot nem üres, Azure AD csatlakozás majd exportálja az objektum Azure AD.
    
 **Megjegyzés:** Egyszer helyszíni AD objektum Azure AD csatlakozás (azaz, importálja a összekötő AD helyet, és a Metaverse vetített) importálja, az sourceAnchor értékét már nem módosíthatja. Adhatja meg a sourceAnchor értékét egy adott helyszíni AD az objektum, az msDS-ConsistencyGuid attribútumot konfigurálása előtt Azure AD csatlakozás lesz importálva. 
  
SourceAnchor és ConsistencyGuid további információt talál a következő: [Azure AD csatlakozás: tervezési koncepciók](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

