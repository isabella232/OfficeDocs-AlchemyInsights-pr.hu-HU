---
title: Az LDAP konfigurálása
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885162"
---
# <a name="configure-ldap"></a>Az LDAP konfigurálása

Az LDAP konfiguráláshoz tegye a következőket:

1. Ellenőrizze tartománya állapotát az [Azure Portal webhelyen.](https://aka.ms/aadds-health)
1. Győződjön meg arról, hogy rendelkezésre áll egy érvényes Azure AD-előfizetés, és hogy engedélyezve van az Azure AD tartományi szolgáltatások.
1. A biztonságos LDAP-hitelesítés engedélyezéséhez szükséges tanúsítványt megbízható hitelesítésszolgáltatótól kell beszerezni, vagy önaírt tanúsítványnak kell lennie.
1. Győződjön meg arról, hogy a tanúsítvány követi a szükséges [irányelveket.](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)

**Érvénytelen tanúsítvány**
1. A tanúsítványok megújításának lépéseit követve hozzon létre egy új tanúsítványt, és töltse újra: Konfigurálja az [LDAP-t.](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
1. Az Azure Active Directory tartományi szolgáltatások biztonságos LDAP-riasztásokkal kapcsolatos ismert problémájának megoldásához lásd: [LDAP-riasztások feloldása.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
