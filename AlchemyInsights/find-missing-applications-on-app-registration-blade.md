---
title: Hiányzó alkalmazások megkeresés az alkalmazás-regisztrációs panelen
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9654"
ms.openlocfilehash: 0dee7e44a8701e1df924b9657cce6cf9d90160e58277d667f6069a4cbcf87ce5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057104"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Hiányzó alkalmazások megkeresés az alkalmazás-regisztrációs panelen

1. Nem találja az alkalmazásregisztrációs portálon található alkalmazásokat.

    Ha egy alkalmazás egy több-bérlős alkalmazás, és egy másik bérlői webhelyen volt regisztrálva, nem jelenik meg az Alkalmazásregisztráció blade felirat alatt. Előfordulhat azonban, hogy az Enterprise Applications blade (Nagyvállalati alkalmazások) panelen találja azt, miután megnyitotta azt (a jóváhagyásukat követően), és létrejött a bérlői webhelyen a szolgáltatásnév. További információt az Alkalmazások és szolgáltatások & Azure [AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)-ban – Microsoft Identitásplatform.
2. Nem lehet megtekinteni az alkalmazásregisztrációk paneljét, még akkor sem, ha Ön rendszergazda.

    Győződjön meg arról, hogy a megfelelő címtárban van az Azure Portal webhelyen.
3. Az alkalmazás nem szerepel az Enterprise Applications blade (Vállalati alkalmazások) panelen, de megjelenik a PowerShell-parancs lekérdező parancsa esetén.

    Néha, miután törölte az alkalmazást az Azure Portalról, az nem jelent meg a portálon, de előfordulhat, hogy nem törlődött teljesen. További információ:
    - A korábban törölt alkalmazások listáját lekérheti, és a **Get-AzureADDeletedApplication** paranccsal láthatja, hogy az alkalmazás megjelenik-e a listában. További információ: [Get-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication)
    - Ha teljesen el szeretné távolítani az alkalmazást, próbálkozzon a következővel a **PowerShellben: Remove-AzureADApplication -ObjectId**. További információ: [Remove-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication).
    - Másik lehetőségként megpróbálhatja visszaállítani a törölt alkalmazást a következő Powershell-paranccsal: **AzureADDeletedApplication -ObjectId visszaállítása.** További információ: [Restore-AzureADDeletedApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
4. Nem találom az összes előre telepített vállalati alkalmazás listáját az új Azure-bérlőben.

    Alapértelmezés szerint nincsenek előre telepített nagyvállalati alkalmazások az Azure AD-ban. Manuálisan kell hozzáadnia az "Új alkalmazás" lehetőségből, ha böngészi az Azure AD gyűjteményből, vagy egy nem galériaalkalmazást ad hozzá. További információt a Rövid útmutató: Alkalmazás hozzáadása a Azure Active Directory [(Azure AD) bérlői webhelyéhez.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)
    Ha Ön globális rendszergazda, az appokat egyszerűen elérheti az Microsoft 365 [appindítóval.](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher)
5. Nem találom az alkalmazásokat a Saját alkalmazások portálon.

    Győződjön meg arról, hogy az alkalmazások nincsenek elrejtve a Saját alkalmazások gyűjteménylapon. További információ: Gyűjtemények [(előzetes verzió) a Saját alkalmazások portálon – Azure AD.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections)
6. Ha alkalmazásokat a Saját alkalmazások portálról & alkalmazások keresését a Saját alkalmazások portálon [– Azure AD webhelyen talál.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access)
7. Office 365 A Mover alkalmazás a telepítés után nem jelenik meg a Nagyvállalati alkalmazások panelen.

    A "Office 365 Mover" egy több-bérlős alkalmazás, amely nem szükséges hozzáadni az AAD-hez a Nagyvállalati app regisztrálása csoport Galériaalkalmazások szakaszában. A Mover Office 365 eléréséhez egyszerűen jelentkezzen be az alkalmazásba, és a felhasználó beleegyezését kéri az engedélyekhez. Miután a felhasználó hozzájárulását adta, ezt az appot a rendszer automatikusan hozzáadja a bérlőhöz azzal az e-mail-azonosítóval, amelybe Ön bejelentkezett.

    Miután bejelentkezik az alkalmazásba, az alkalmazás bejegyzését megtalálja az AAD Enterprise Applications blade (Nagyvállalati alkalmazások) panelje alatt. Az alkalmazás teljes nevének (például "Office 365 Mover) beírásával vagy egyszerűen az "office" kifejezésre keresve meg kell keresnie az alkalmazást. További információt a Mover Office 365, amely szerint a Mover már telepítve van, de nem szerepel a Nagyvállalati alkalmazások [gyűjteményében.](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)
8. [Rövid útmutató: Az Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) bérlői webhelyet identitáskezelésre használó alkalmazások listájának megtekintése bemutatja, hogy miként használhatja az Azure AD-bérlőt identitásszolgáltatóként már beállított alkalmazások, más néven appok megtekintéséhez.
9. [Az alkalmazások hozzáadásakor](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) vagy eltávolításakor a Azure Active Directory segít megérteni, hogy a felhasználók milyen gyakori problémákkal szembesülnek az alkalmazások Azure Active Directory.
