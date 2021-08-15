---
title: Upn sync disabled
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
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: fc163fae4d348d7c7cf117bd457f999b42f96bec7c1eb9aa1435e346131d06de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038114"
---
# <a name="upn-sync-disabled"></a>Upn sync disabled

Ha 2016. március 30. előtt kezdte el a szinkronizálást az Azure AD-be, az alábbi Azure AD PowerShell-parancsmag futtatásával engedélyezze az upn soft matcht csak a szervezet számára:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
Az upn szoftveres egyezés automatikusan be van kapcsolva az Azure AD-re 2016. március 30-án vagy azt követően szinkronizáló szervezeteknél.
  
Ha szeretne többet megtudni a szoftveres egyezés upn-hez és más szinkronizálási funkciókhoz való engedélyezéséről, olvassa el az [Azure AD Csatlakozás szinkronizálási szolgáltatás funkcióit.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

