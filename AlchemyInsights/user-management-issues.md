---
title: Felhasználókezelési problémák
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036283"
---
# <a name="user-management-issues"></a>Felhasználókezelési problémák

**Mi történik az alkalmazáshoz aktuálisan hozzárendelt felhasználókkal, ha letiltom a "Felhasználói hozzárendelés szükséges" tulajdonságot (a tulajdonságot állítsa Nemre) ?**

Ha **letiltja a felhasználói hozzárendelést,** az nincs hatással az aktuálisan hozzárendelt felhasználókra. Ha letiltja ezt a tulajdonságot, az csak az összes felhasználónak engedélyezi az alkalmazáshoz való hozzáférést. Az alkalmazásban a felsorolt felhasználók és a csoportokhoz rendelt felhasználók továbbra is érvényesek maradnak.

- Ha adott felhasználókészletre korlátozná az appot, tekintse meg az Azure AD-app felhasználók egy bizonyos halmazára való korlátozását [– Microsoft-identitásplatform | Microsoft Docs .](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.)
- Ha felhasználókat és csoportokat szeretne hozzárendelni a nagyvállalati alkalmazásokhoz az Azure Active Directoryban (Azure AD), akár az Azure Portalon belül, akár a PowerShell használatával, tekintse meg az Alkalmazás felhasználói hozzárendelésének kezelése az [Azure Active Directorybancímű](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal)részt.
- Az alkalmazáskészítési és -kezelési engedélyek delegálhatóak: Alkalmazáskezelési rendszergazdai engedélyek [delegálása – Azure AD | Microsoft Docs .](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles)
- **Adott nagyvállalati alkalmazások elrejtése a** felhasználók elől – Az alábbi lépésekkel elrejtheti az összes Microsoft 365-appot a **MyApps panelről.** Az appok továbbra is láthatók maradnak az Office 365 portálon.

 1. Jelentkezzen be az Azure Portalba a címtár globális rendszergazdájaként. 
 2. Válassza **az Azure Active Directory lehetőséget.** 
 3. Válassza a **Felhasználók** lehetőséget. 
 4. Válassza **a Felhasználói beállítások lehetőséget.** 
 5. A **Nagyvállalati alkalmazások csoportban** kattintson a Végfelhasználók indításának és megtekintésének **kezelése elemre.** 
 6. A **felhasználók csak az Office 365-appokat** láthatják az Office 365 portálon, kattintson az Igen **gombra.** 
 7. Kattintson a **Mentés** gombra. 
 8. További információt a Nagyvállalati alkalmazás elrejtése a felhasználói felület elől az [Azure AD-| Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)

- Ha számos szervezetnek kínál Szoftverszolgáltatásként (SaaS-) alkalmazást, konfigurálhatja úgy az alkalmazást, hogy bármely Azure Active Directory (Azure AD) bérlői fiókból fogadjon bejelentkezéseket. Ezt a konfigurációt "az alkalmazás több-bérlősként" nevezik. Az Azure AD-bérlők felhasználói bejelentkeznek az appba, miután hozzájárultak ahhoz, hogy az appban használják a fiókjukat. További információt Az Azure AD-felhasználókkal bejelentkező alkalmazások – [Microsoft-identitásplatform és a Microsoft-identitásplatform | Microsoft Docs .](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant)

- **Hogyan férhetnek hozzá a végfelhasználók az alkalmazáshoz, miután hozzárendelték az alkalmazáshoz?**

A Nagyvállalati verziós alkalmazások minden appja rendelkezik egy hivatkozással, amely a végfelhasználók számára elérhető. A felhasználók a **Myapps** portálon keresztül is egyszerűen elérhetik az appot.

- **Tudni szeretné, hogy a felhasználók mely alkalmazásokat és alkalmazástípusokat használják?**

Az elmúlt 30 nap bejelentkezési jelentéseit letöltheti az Azure Active Directoryból portal.azure.com > Bejelentkezések>> **jelentéseket.**

- Megtudhatja, hogyan [adhat bérlői szintű](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) rendszergazdai hozzájárulást egy alkalmazáshoz, és hogyan konfigurálhatja a végfelhasználók által [az alkalmazásokhoz való hozzájárulást.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent)

- A hozzájárulás [működése és az](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) [alkalmazásokhoz való hozzájárulás kezelése.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests)


