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
ms.openlocfilehash: 2b1ba772459091ce1a796884997fe2516d0407eb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782153"
---
# <a name="upn-sync-disabled"></a>Upn sync disabled

Ha 2016. március 30. előtt kezdte el a szinkronizálást az Azure AD-be, az alábbi Azure AD PowerShell-parancsmag futtatásával engedélyezze az upn soft matcht csak a szervezet számára:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
Az upn szoftveres egyezés automatikusan be van kapcsolva az Azure AD-re 2016. március 30-án vagy azt követően szinkronizáló szervezeteknél.
  
A szoftveres egyezés UPN-hez és más szinkronizálási funkciókhoz való engedélyezéséről további információt Az Azure AD Connect szinkronizálási szolgáltatás [szolgáltatásairól olvashat.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

