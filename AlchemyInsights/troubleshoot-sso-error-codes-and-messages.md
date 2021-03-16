---
title: A zökkenőmentes egyszeri bejelentkezéssel kapcsolatos hibakódok és üzenetek elhárítása
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9367"
- "9004357"
ms.openlocfilehash: 805a85ffd47e14295c375fc415301570de22bfd8
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816215"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-error-codes-and-messages"></a><span data-ttu-id="ef7cf-102">A zökkenőmentes egyszeri bejelentkezéssel kapcsolatos hibakódok és üzenetek elhárítása</span><span class="sxs-lookup"><span data-stu-id="ef7cf-102">Troubleshoot Seamless Single Sign-on (SSO) error codes and messages</span></span>

<span data-ttu-id="ef7cf-103">A zökkenőmentes egyszeri bejelentkezéssel kapcsolatos hibakódok és üzenetek megoldásához végezze el az alábbi lépéseket:</span><span class="sxs-lookup"><span data-stu-id="ef7cf-103">To resolve Seamless Single Sign-on (SSO) error codes and messages, perform the following steps:</span></span>

1. <span data-ttu-id="ef7cf-104">Tekintse át és hárítsa el az SSO-hibákat az Azure Active Directory portál bejelentkezési [tevékenységjelentéseiben.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins)</span><span class="sxs-lookup"><span data-stu-id="ef7cf-104">Review and troubleshoot SSO errors by going to the [Sign-in activity reports in the Azure Active Directory portal](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins).</span></span>
2. <span data-ttu-id="ef7cf-105">Lásd: Az [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#sign-in-failure-reasons-in-the-azure-active-directory-admin-center-needs-a-premium-license) közvetlen egyszeri bejelentkezéssel kapcsolatos hibáinak elhárítása – Ez a cikk segítséget nyújt az Azure Active Directory (Azure AD Sign-On) zökkenőmentes egyszeri bejelentkezési szolgáltatásával kapcsolatos gyakori problémák hibaelhárításához.</span><span class="sxs-lookup"><span data-stu-id="ef7cf-105">See [Troubleshoot Azure Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#sign-in-failure-reasons-in-the-azure-active-directory-admin-center-needs-a-premium-license) - This article helps you find troubleshooting information about common problems regarding Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO).</span></span>
3. <span data-ttu-id="ef7cf-106">Lásd [az Azure AD authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#lookup-current-error-code-information) (Azure AD-hitelesítési és engedélyezési hibakódok) – Ez a cikk segítséget nyújt az Azure Active Directory (Azure AD) biztonsági jogkivonat-szolgáltatásból visszaadott AADSTS-hibakódok megkeresése során.</span><span class="sxs-lookup"><span data-stu-id="ef7cf-106">See [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#lookup-current-error-code-information) - This article helps you find information about the AADSTS error codes that are returned from the Azure Active Directory (Azure AD) security token service (STS).</span></span> <span data-ttu-id="ef7cf-107">Ez a cikk az AADSTS-hibák leírásának, javításának és néhány javasolt kerülő megoldásának megkeresésében is segítséget nyújt.</span><span class="sxs-lookup"><span data-stu-id="ef7cf-107">This article also helps you find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>

<span data-ttu-id="ef7cf-108">[Microsoft kérdések&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) – Ebből a cikkből többet is talál a zökkenőmentes egyszeri bejelentkezésről, ha szolgáltatáskéréseket vagy technikai kérdéseket kell feltennie.</span><span class="sxs-lookup"><span data-stu-id="ef7cf-108">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - See this article for information on making feature requests or asking technical questions about Seamless SSO.</span></span>

