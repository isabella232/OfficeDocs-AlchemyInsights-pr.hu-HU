---
title: Jelszó kivonatszinkronizálása a tartományszolgáltatáshoz
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177489"
---
# <a name="password-hash-synchronization-for-domain-service"></a>Jelszó kivonatszinkronizálása a tartományszolgáltatáshoz

**Ha az Azure AD DS-példánya jelszó-kivonat-szinkronizálás engedélyezését kéri**

Olyan helyzettel találkozhat, amelyben hibrid környezetet futtat, amelyben a felhasználók helyszíni Azure Active Directory tartományi szolgáltatások (AD DS) környezetből szinkronizálnak. Ez a helyzet annak ellenére merül fel, hogy jelszó-kivonat-szinkronizálást használ a helyszíni AD DS-ről az Azure AD-bérlőjébe.

**A probléma oka**

Ennek az az oka, hogy az Azure AD Connect alapértelmezés szerint nem szinkronizálja az Azure AD DS-hez szükséges régi New Technology LAN Manager -előfizetéseket és Kerberos-jelszavakat.

**Kerülő megoldás** 

Konfigurálnia kell az Azure AD Connectet az NTLM- és Kerberos-hitelesítéshez szükséges jelszó-előjelszavak szinkronizálásához.

Miután konfigurálta az Azure AD Connectet, egy helyszíni fiók létrehozása vagy jelszó-módosítási esemény is szinkronizálja a régi jelszó-előjeleket az Azure AD-be. Erről [és](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) arról, hogy miként engedélyezheti a jelszó-szinkronizálást az Azure AD DS hibrid környezetében, olvassa el itt a további információkat.