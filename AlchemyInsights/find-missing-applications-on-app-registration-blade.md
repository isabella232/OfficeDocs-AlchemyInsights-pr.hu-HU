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
ms.openlocfilehash: 00b5821e2edad8b60ff60b1f85264d81c72277e4
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404695"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Hiányzó alkalmazások megkeresés az alkalmazás-regisztrációs panelen

1. Nem találja az alkalmazásregisztrációs portálon található alkalmazásokat.

    Ha egy alkalmazás egy több-bérlős alkalmazás, és egy másik bérlői webhelyen volt regisztrálva, nem jelenik meg az Alkalmazásregisztráció blade felirat alatt. Előfordulhat azonban, hogy az Enterprise Applications blade (Nagyvállalati alkalmazások) panelen találja azt, miután megnyitotta azt (a jóváhagyásukat követően), és létrejött a bérlői webhelyen a szolgáltatásnév. További információt az Alkalmazások és szolgáltatások & Azure [AD – Microsoft-identitásplatform szolgáltatásban.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
2. Nem lehet megtekinteni az alkalmazásregisztrációk paneljét, még akkor sem, ha Ön rendszergazda.

    Győződjön meg arról, hogy a megfelelő címtárban van az Azure Portal webhelyen.
3. Az alkalmazás nem szerepel az Enterprise Applications blade (Vállalati alkalmazások) panelen, de megjelenik a PowerShell-parancs lekérdező parancsa esetén.

    Néha, miután törölte az alkalmazást az Azure Portalról, az nem jelent meg a portálon, de előfordulhat, hogy nem törlődött teljesen. További információ:
    - A korábban törölt alkalmazások listáját lekérheti, és a **Get-AzureADDeletedApplication** paranccsal láthatja, hogy az alkalmazás megjelenik-e a listában. További információ: [Get-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication)
    - Ha teljesen el szeretné távolítani az alkalmazást, próbálkozzon a következővel a **PowerShellben: Remove-AzureADApplication -ObjectId**. További információ: [Remove-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication).
    - Másik lehetőségként megpróbálhatja visszaállítani a törölt alkalmazást a következő Powershell-paranccsal: **AzureADDeletedApplication -ObjectId visszaállítása.** További információ: [Restore-AzureADDeletedApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
4. Nem találom az összes előre telepített vállalati alkalmazás listáját az új Azure-bérlőben.

    Alapértelmezés szerint nincsenek előre telepített nagyvállalati alkalmazások az Azure AD-ban. Manuálisan kell hozzáadnia az "Új alkalmazás" lehetőségből, ha böngészi az Azure AD gyűjteményből, vagy egy nem galériaalkalmazást ad hozzá. További információt a Rövid útmutató: Alkalmazás hozzáadása Az [Azure Active Directory (Azure AD) bérlői webhelyéhez.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)
    Ha Ön globális rendszergazda, egyszerűen elérheti az appokat a [Microsoft 365 appindítójával.](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher)
5. Nem találom az alkalmazásokat a Saját alkalmazások portálon.

    Győződjön meg arról, hogy az alkalmazások nincsenek elrejtve a Saját alkalmazások gyűjteménylapon. További információ: Gyűjtemények [(előzetes verzió) a Saját alkalmazások portálon – Azure AD.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections)
6. Ha alkalmazásokat a Saját alkalmazások portálról & alkalmazások keresését a Saját alkalmazások portálon [– Azure AD webhelyen talál.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access)
7. Az Office 365 Mover app telepítés után nem jelenik meg a Nagyvállalati alkalmazások panelen.

    Az "Office 365 Mover" alkalmazás egy több-bérlős app, és nem szükséges hozzáadni az AAD-hez a Nagyvállalati app regisztrálása csoport Galériaalkalmazások szakaszában. Az Office 365 Mover app eléréséhez egyszerűen jelentkezzen be az appba, és a felhasználó beleegyezését kéri az engedélyekhez. Miután a felhasználó hozzájárulását adta, ezt az appot a rendszer automatikusan hozzáadja a bérlőhöz azzal az e-mail-azonosítóval, amelybe Ön bejelentkezett.

    Miután bejelentkezik az alkalmazásba, az alkalmazás bejegyzését megtalálja az AAD Enterprise Applications blade (Nagyvállalati alkalmazások) panelje alatt. Az alkalmazás teljes nevének (office 365 Mover) beírásával vagy egyszerűen az "office" szóra keresve kell keresnie. További információ: [Az Office 365 Mover](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)azt mondja, hogy az már telepítve van, de nem szerepel a Nagyvállalati alkalmazások gyűjteményében.
8. [Rövid útmutató: Az Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) bérlői webhelyet identitáskezelésre használó alkalmazások listájának megtekintése bemutatja, hogy miként használhatja az Azure AD-bérlőt identitásszolgáltatóként már beállított alkalmazások, más néven appok megtekintéséhez.
9. [Az alkalmazások Azure Active Directoryba](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) való felvételével vagy eltávolításával kapcsolatos gyakori problémák elhárítása segít megérteni az alkalmazásokat az Azure Active Directoryban megtekintő gyakori problémákat.
