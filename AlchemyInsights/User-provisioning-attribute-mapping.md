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
# <a name="user-provisioning-attribute-mapping"></a>Felhasználó kiépítési attribútumának megfeleltetése

1. Az attribútumleképezéssel kapcsolatos ismert problémák elhárításáról az [Attribútumleképezések témakörben kaphat további hibaelhárítást.](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings) 
2. A Microsoft Azure Active Directory (AD) támogatást nyújt külső SaaS-alkalmazások , például a Salesforce, a G Suite és mások számára történő felhasználói kiépítéshez. Ha engedélyezi egy külső SaaS-alkalmazás felhasználói jogosultságkiosztását, az Azure Portal az attribútumértékeket attribútumleképezések segítségével szabályozza. Az alapértelmezett attribútumleképezések testreszabását az Azure Active Directoryban használt [SaaS-alkalmazások](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes)felhasználói kiépítési attribútumleképezésének testreszabása.
    - Ha szeretne többet megtudni a SaaS-appok felhasználóinak kiépítésekor, olvassa el a ["Mi az automatikus SaaS-appok kiépítése az Azure AD-ban?"](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning) 
3. Amikor testre szabja az attribútum-leképezéseket a felhasználói kiépítéshez, előfordulhat, hogy a megfeleltetni kívánt attribútum nem jelenik meg a Forrás attribútumlistában. A helyszíni Active Directoryból származó attribútum szinkronizálása az [Azure AD-hez](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) egy alkalmazásbeli cikkhez való kiépítéshez azt mutatja be, hogy miként adjuk hozzá a hiányzó attribútumot úgy, hogy szinkronizáljuk azt a helyszíni AD-ről az Azure AD-be.
