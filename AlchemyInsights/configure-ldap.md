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
ms.openlocfilehash: 3f1f9728cdcfbe5676e5afc45b2afe82836fed9c8907df3559ac7daec21194ed
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090414"
---
# <a name="configure-ldap"></a>Az LDAP konfigurálása

Az LDAP beállításhoz tegye a következőket:

1. Ellenőrizze tartománya állapotát az [Azure Portal webhelyen.](https://aka.ms/aadds-health)
1. Győződjön meg arról, hogy rendelkezésre áll egy érvényes Azure AD-előfizetés, és hogy engedélyezve van az Azure AD tartományi szolgáltatások.
1. A biztonságos LDAP engedélyezéséhez szükséges tanúsítványt megbízható hitelesítésszolgáltatótól vagy önaírt tanúsítványból kell beszerezni.
1. Győződjön meg arról, hogy a tanúsítvány követi a szükséges [irányelveket.](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)

**Érvénytelen tanúsítvány**
1. A tanúsítványok megújításának lépéseit követve hozzon létre egy új tanúsítványt, és töltse újra: [Az LDAP konfigurálása.](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
1. A Biztonságos LDAP-riasztásokkal kapcsolatos ismert problémák megoldása az Azure Active Directory tartományi szolgáltatásokban: [LDAP-riasztások feloldása.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
