---
title: Nagyvállalati alkalmazások listájának lekérte
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
- "9004342"
- "9837"
ms.openlocfilehash: 99e4f7e676610103355736ce847930c6c5d2d7532c4756ac4551a8d9b3020176
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54116730"
---
# <a name="get-a-list-of-enterprise-applications"></a>Nagyvállalati alkalmazások listájának lekérte

1. Ha a Powershell-parancson keresztül le kell szereznie **a** vállalati alkalmazások listáját (minden alkalmazást, vagy a Megjelenítendő név, azonosító, Azonosító URI-k stb. szerint szűrve), lásd: [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).
2. Ha az egyszerű szolgáltatásobjektumok listáját (az összes objektumot vagy az azonosító alapján szűrt objektumokat) a Powershell-parancson keresztül, lásd: [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).
3. Ha le szeretné kérni **a konfigurált SAML-appok listáját,** a PowerShell-parancsprogramokat követő parancsprogramokkal segítséget tud kapni:

    Minden alkalmazás legyen OAuth- vagy SAML-app (gyűjtemény- és nem galériaalkalmazások egyaránt) két objektumot hozna létre az AAD-ban regisztrációkor. Az egyik az Application objektum, a másik pedig a Service Principal objektum. Amikor egy egyszerű szolgáltatásobjektum tulajdonságait a PowerShell használatával kiradhozta, azt fogja találni, hogy minden alkalmazáshoz adott számú címke van társítva, például:

    - Az OAuth-appok címkéje **"WindowsAzureActiveDirectoryIntegratedApp"** lenne.
    - Az SAML-appok galériában a **"WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1"** címkét kellene megjelölni.
    - A nem galériaként használt SAML-appok címkéje **"WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"

    Ezért ezeket a címkéket használva kiderítheti, hogy milyen típusú az app. A **"WindowsAzureActiveDirectoryIntegratedApp"** címke minden apptípusnál gyakori. Az alábbi kódrészletet használva felsorolhatja az összes SAML-appot (a galériát és a nem galériát is):

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    További információ: [AZ SAML-kompatibilis alkalmazások azonosítása az Azure AD-ban.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)

4. **Csak a webalkalmazások** kereséséhez és listához: Az alábbi paranccsal szerezze be az összes Azure AD-alkalmazást a "Web app/API" alkalmazástípussal.

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT
5. **Csak a natív alkalmazások megkereséséről** és listáról: Futtassa az alábbi parancsot az összes natív ügyfélalkalmazás (asztali/mobileszköz) alkalmazás be szerezze be.

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT
6. **Az összes regisztrált Azure AD-alkalmazás részleteinek** exportálása CSV-fájlba: Az alábbi parancs exportálja az összes Azure AD-appot a szükséges adatokkal a CSV-fájlba:

    - Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8

7. **Exportálni kell a nem használt Azure-appok listáját** – Naplójelentés

    Az Azure AD legfeljebb 30 napig képes az alkalmazásnaplók megtekintésére, feltéve, hogy rendelkezik prémium szintű Azure AD licenccel.
    Két lehetőség közül választhat, hogy 30 napnál tovább megőrizze az adatokat. Az Azure [AD reporting API-k](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) használatával programozással beolvashatja és adatbázisba tárolhatja az adatokat. Másik lehetőségként integrálhatja az auditnaplókat egy külső SIEM-rendszerbe.

    Az összes alkalmazás és tulajdonú alkalmazás applistát letöltheti az Azure Active Directory>alkalmazás-regisztrációk>Az összes alkalmazás/tulajdonú alkalmazás letöltése>alatt.

    Az alkalmazások MS Graph-ön keresztüli listáját a Listaalkalmazások [– Microsoft Graph 1.0-s](https://docs.microsoft.com/graph/api/application-list) és alkalmazáserőforrás-típusa [– Microsoft Graph 1.0](https://docs.microsoft.com/graph/api/resources/application).
