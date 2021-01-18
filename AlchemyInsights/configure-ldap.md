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
# <a name="configure-ldap"></a><span data-ttu-id="cf963-102">Az LDAP konfigurálása</span><span class="sxs-lookup"><span data-stu-id="cf963-102">Configure LDAP</span></span>

<span data-ttu-id="cf963-103">Az LDAP konfiguráláshoz tegye a következőket:</span><span class="sxs-lookup"><span data-stu-id="cf963-103">To configure LDAP, do the following:</span></span>

1. <span data-ttu-id="cf963-104">Ellenőrizze tartománya állapotát az [Azure Portal webhelyen.](https://aka.ms/aadds-health)</span><span class="sxs-lookup"><span data-stu-id="cf963-104">Check your domain’s health on the [Azure portal](https://aka.ms/aadds-health).</span></span>
1. <span data-ttu-id="cf963-105">Győződjön meg arról, hogy rendelkezésre áll egy érvényes Azure AD-előfizetés, és hogy engedélyezve van az Azure AD tartományi szolgáltatások.</span><span class="sxs-lookup"><span data-stu-id="cf963-105">Ensure a valid Azure AD subscription is available and Azure AD Domain Services has been enabled.</span></span>
1. <span data-ttu-id="cf963-106">A biztonságos LDAP-hitelesítés engedélyezéséhez szükséges tanúsítványt megbízható hitelesítésszolgáltatótól kell beszerezni, vagy önaírt tanúsítványnak kell lennie.</span><span class="sxs-lookup"><span data-stu-id="cf963-106">The certificate required to enable secure LDAP must be obtained from a trusted public certification authority or be a self-signed certificate.</span></span>
1. <span data-ttu-id="cf963-107">Győződjön meg arról, hogy a tanúsítvány követi a szükséges [irányelveket.](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)</span><span class="sxs-lookup"><span data-stu-id="cf963-107">Ensure the certificate follows the required [guidelines](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span></span>

<span data-ttu-id="cf963-108">**Érvénytelen tanúsítvány**</span><span class="sxs-lookup"><span data-stu-id="cf963-108">**Invalid Certificate**</span></span>
1. <span data-ttu-id="cf963-109">A tanúsítványok megújításának lépéseit követve hozzon létre egy új tanúsítványt, és töltse újra: Konfigurálja az [LDAP-t.](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="cf963-109">To renew a certificate, follow the steps to create a new certificate and reupload: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
1. <span data-ttu-id="cf963-110">Az Azure Active Directory tartományi szolgáltatások biztonságos LDAP-riasztásokkal kapcsolatos ismert problémájának megoldásához lásd: [LDAP-riasztások feloldása.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="cf963-110">To resolve known issue with Secure LDAP alerts in Azure Active directory Domain Services, see [Resolve LDAP alerts](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
