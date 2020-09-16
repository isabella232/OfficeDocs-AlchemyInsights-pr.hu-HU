---
title: Egyszerű UPN-szinkronizálás letiltva
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
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749516"
---
# <a name="upn-sync-disabled"></a>Egyszerű UPN-szinkronizálás letiltva

Ha az Azure AD-hoz való szinkronizálást a március 30-án, 2016-ban futtatja, futtassa a következő Azure AD PowerShell-parancsmagot, és csak akkor engedélyezze a szervezetnek az egyszerű felhasználónevet:
  
 **Set-MsolDirSyncFeature-EnableSoftMatchOnUpn funkció engedélyezése $True**
  
Az UPN-alapú Soft-egyezés automatikusan be van kapcsolva azoknál a szervezetekben, amelyek az Azure AD-on való szinkronizálást kezdték el, illetve március 30, 2016
  
Ha többet szeretne megtudni arról, hogy miként engedélyezheti a Soft-egyezést az UPN-és egyéb szinkronizálási funkciókhoz, olvassa el az [Azure ad Connect szinkronizálási szolgáltatás](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

