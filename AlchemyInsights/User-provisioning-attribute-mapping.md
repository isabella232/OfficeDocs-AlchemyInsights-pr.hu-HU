---
title: Felhasználó kiépítési attribútumának megfeleltetése
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949764"
---
# <a name="user-provisioning-attribute-mapping"></a><span data-ttu-id="71dd2-102">Felhasználó kiépítési attribútumának megfeleltetése</span><span class="sxs-lookup"><span data-stu-id="71dd2-102">User-provisioning attribute mapping</span></span>

1. <span data-ttu-id="71dd2-103">Az attribútumleképezéssel kapcsolatos ismert problémák elhárításáról az [Attribútumleképezések témakörben kaphat további hibaelhárítást.](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings)</span><span class="sxs-lookup"><span data-stu-id="71dd2-103">To troubleshoot known attribute-mapping issues, see [Attribute mappings](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span></span> 
2. <span data-ttu-id="71dd2-104">A Microsoft Azure Active Directory (AD) támogatást nyújt külső SaaS-alkalmazások , például a Salesforce, a G Suite és mások számára történő felhasználói kiépítéshez.</span><span class="sxs-lookup"><span data-stu-id="71dd2-104">Microsoft Azure Active Directory (AD) provides support for user provisioning to third-party SaaS applications such as Salesforce, G Suite and others.</span></span> <span data-ttu-id="71dd2-105">Ha engedélyezi egy külső SaaS-alkalmazás felhasználói jogosultságkiosztását, az Azure Portal az attribútumértékeket attribútumleképezések segítségével szabályozza.</span><span class="sxs-lookup"><span data-stu-id="71dd2-105">If you enable user provisioning for a third-party SaaS application, the Azure portal controls its attribute values through attribute-mappings.</span></span> <span data-ttu-id="71dd2-106">Az alapértelmezett attribútumleképezések testreszabását az Azure Active Directoryban használt [SaaS-alkalmazások](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes)felhasználói kiépítési attribútumleképezésének testreszabása.</span><span class="sxs-lookup"><span data-stu-id="71dd2-106">To learn how to customize the default attribute-mappings, see [Customize user provisioning attribute-mappings for SaaS applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span></span>
    - <span data-ttu-id="71dd2-107">Ha szeretne többet megtudni a SaaS-appok felhasználóinak kiépítésekor, olvassa el a ["Mi az automatikus SaaS-appok kiépítése az Azure AD-ban?"](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span><span class="sxs-lookup"><span data-stu-id="71dd2-107">To learn more about SaaS app user provisioning, see [What is automated SaaS app user provisioning in Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span></span> 
3. <span data-ttu-id="71dd2-108">Amikor testre szabja az attribútum-leképezéseket a felhasználói kiépítéshez, előfordulhat, hogy a megfeleltetni kívánt attribútum nem jelenik meg a Forrás attribútumlistában.</span><span class="sxs-lookup"><span data-stu-id="71dd2-108">When customizing attribute-mappings for user provisioning, you might find that the attribute you want to map doesn't appear in the Source attribute list.</span></span> <span data-ttu-id="71dd2-109">A helyszíni Active Directoryból származó attribútum szinkronizálása az [Azure AD-hez](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) egy alkalmazásbeli cikkhez való kiépítéshez azt mutatja be, hogy miként adjuk hozzá a hiányzó attribútumot úgy, hogy szinkronizáljuk azt a helyszíni AD-ről az Azure AD-be.</span><span class="sxs-lookup"><span data-stu-id="71dd2-109">The [Sync an attribute from your on-premises Active Directory to Azure AD for provisioning to an application](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) article shows you how to add the missing attribute by synchronizing it from your on-premises AD to Azure AD.</span></span>
