---
title: Upn szinkronizálás letiltva
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
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 33bc7e30d41ff70e2ce55d946202acf45dbcb0f2
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726106"
---
# <a name="upn-sync-disabled"></a>Upn szinkronizálás letiltva

Ha 2016. március 30-a előtt kezdte meg a szinkronizálást az Azure AD szolgáltatással, futtassa a következő Azure AD PowerShell-parancsmast, hogy csak a szervezet számára engedélyezze az UPN-alapú lágy egyezést:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Engedélyezés $True**
  
Az UPN soft match automatikusan be van kapcsolva azon szervezetek esetében, amelyek 2016.
  
Ha többet szeretne tudni arról, hogy miként engedélyezte a soft match funkciót az upn és más szinkronizálási funkciókban, olvassa el az [Azure AD Connect szinkronizálási szolgáltatásának funkcióit.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

