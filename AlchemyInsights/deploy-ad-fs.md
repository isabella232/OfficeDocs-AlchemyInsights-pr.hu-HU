---
title: Az AD FS üzembe helyezése
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1300012"
- "7420"
ms.openlocfilehash: a304504f7483036884878639dfa6ebfc3cdfcac8
ms.sourcegitcommit: 05a9dd3121c21322dc9ddec4c2eec548cafd5a43
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177545"
---
# <a name="deploy-ad-fs"></a><span data-ttu-id="c210f-102">Az AD FS üzembe helyezése</span><span class="sxs-lookup"><span data-stu-id="c210f-102">Deploy AD FS</span></span>

<span data-ttu-id="c210f-103">Az Active Directory összevonási szolgáltatások (AD FS) telepítése a helyszíni infrastruktúrát használja az Office 365-szolgáltatások felhasználóinak hitelesítésére.</span><span class="sxs-lookup"><span data-stu-id="c210f-103">An Active Directory Federation Services (AD FS) deployment uses your on-premises infrastructure to authenticate users for ‎Office 365 services.</span></span> <span data-ttu-id="c210f-104">Összevont bejelentkezéssel engedélyezheti a felhasználóknak, hogy az Azure Active Directoryval (Azure AD) integrált Szolgáltatásként (SAAS) bejelentkezve jelentkezzenek be az Office 365-szolgáltatásokba és -szoftverekbe.</span><span class="sxs-lookup"><span data-stu-id="c210f-104">With federated sign-in, you can enable users to sign in to Office 365 services and Software as a Service (SAAS) applications that are integrated with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="c210f-105">Az összevont bejelentkezés hitelesíti a felhasználókat a helyszíni Active Directory-címtárban az AD FS szolgáltatáson keresztül.</span><span class="sxs-lookup"><span data-stu-id="c210f-105">Federated sign-in authenticates users against your on-premises Active Directory via AD FS.</span></span> <span data-ttu-id="c210f-106">Emellett a vállalati hálózaton a felhasználóknak nem kell újra megadniuk a jelszavukat.</span><span class="sxs-lookup"><span data-stu-id="c210f-106">Also, while on the corporate network, users won't be required to reenter their passwords.</span></span>

<span data-ttu-id="c210f-107">Az [AD FS](https://go.microsoft.com/fwlink/?linkid=2071178) üzembe helyezési tanácsadója részletes útmutatást nyújt egy helyszíni AD FS-infrastruktúra telepítéséhez, amely hitelesíti a felhasználókat a Microsoft 365 és az Office 365 szolgáltatásaihoz.</span><span class="sxs-lookup"><span data-stu-id="c210f-107">The [AD FS deployment advisor](https://go.microsoft.com/fwlink/?linkid=2071178) provides you with step-by-step guidance on deploying an on-premises AD FS infrastructure that authenticates users for Microsoft 365 and Office 365 services.</span></span> <span data-ttu-id="c210f-108">Ezzel az útmutatóval a szervezet áttekintheti az AD FS összetevőit és követelményeit, a telepítéshez szükséges SSL-tanúsítványokat szerezhet be és telepíthet, valamint telepíthet egy szükséges webalkalmazás-proxykiszolgálót.</span><span class="sxs-lookup"><span data-stu-id="c210f-108">With this guide, your organization can review AD FS components and requirements, acquire and install SSL certificates that are necessary for deployment, and install a required web application proxy server.</span></span>
