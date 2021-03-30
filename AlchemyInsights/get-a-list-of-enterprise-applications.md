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
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/26/2021
ms.locfileid: "51404930"
---
# <a name="get-a-list-of-enterprise-applications"></a><span data-ttu-id="34c79-102">Nagyvállalati alkalmazások listájának lekérte</span><span class="sxs-lookup"><span data-stu-id="34c79-102">Get a list of Enterprise Applications</span></span>

1. <span data-ttu-id="34c79-103">Ha a Powershell-parancson keresztül le kell szereznie **a** vállalati alkalmazások listáját (minden alkalmazást, vagy a Megjelenítendő név, azonosító, Azonosító URI-k stb. szerint szűrve), lásd: [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span><span class="sxs-lookup"><span data-stu-id="34c79-103">To **get a list of enterprise applications** (all applications or filtered by Display name, ID, Identifier URIs, etc.) through Powershell command, see [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span></span>
2. <span data-ttu-id="34c79-104">Ha az egyszerű szolgáltatásobjektumok listáját (az összes objektumot vagy az azonosító alapján szűrt objektumokat) a Powershell-parancson keresztül, lásd: [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span><span class="sxs-lookup"><span data-stu-id="34c79-104">To get a list of service principal objects (all objects or filtered by ID) through Powershell command, see [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span></span>
3. <span data-ttu-id="34c79-105">Ha le szeretné kérni **a konfigurált SAML-appok listáját,** a PowerShell-parancsprogramokat követő parancsprogramokkal segítséget tud kapni:</span><span class="sxs-lookup"><span data-stu-id="34c79-105">If you want to **get a list of SAML configured apps, following PowerShell scripts** may help you:</span></span>

    <span data-ttu-id="34c79-106">Minden alkalmazás legyen OAuth- vagy SAML-app (gyűjtemény- és nem galériaalkalmazások egyaránt) két objektumot hozna létre az AAD-ban regisztrációkor.</span><span class="sxs-lookup"><span data-stu-id="34c79-106">Every Application be it an OAuth app or SAML app (both gallery and non-gallery apps) would have two objects created in AAD when their registration happens.</span></span> <span data-ttu-id="34c79-107">Az egyik az Application objektum, a másik pedig a Service Principal objektum.</span><span class="sxs-lookup"><span data-stu-id="34c79-107">One is called the Application Object and the other is the Service Principal object.</span></span> <span data-ttu-id="34c79-108">Amikor egy egyszerű szolgáltatásobjektum tulajdonságait a PowerShell használatával kiradhozta, azt fogja találni, hogy minden alkalmazáshoz adott számú címke van társítva, például:</span><span class="sxs-lookup"><span data-stu-id="34c79-108">When you dump the properties of a Service Principal Object using PowerShell, you would find that every application has a certain number of Tags associated with it like:</span></span>

    - <span data-ttu-id="34c79-109">Az OAuth-appok címkéje **"WindowsAzureActiveDirectoryIntegratedApp"** lenne.</span><span class="sxs-lookup"><span data-stu-id="34c79-109">OAuth apps would have a tag called "**WindowsAzureActiveDirectoryIntegratedApp**"</span></span>
    - <span data-ttu-id="34c79-110">Az SAML-appok galériában a **"WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1"** címkét kellene megjelölni.</span><span class="sxs-lookup"><span data-stu-id="34c79-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span></span>
    - <span data-ttu-id="34c79-111">A nem galériaként használt SAML-appok címkéje **"WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span><span class="sxs-lookup"><span data-stu-id="34c79-111">Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span></span>

    <span data-ttu-id="34c79-112">Ezért ezeket a címkéket használva kiderítheti, hogy milyen típusú az app.</span><span class="sxs-lookup"><span data-stu-id="34c79-112">Hence, you can use these tags and find out what kind of app it is.</span></span> <span data-ttu-id="34c79-113">A **"WindowsAzureActiveDirectoryIntegratedApp"** címke minden apptípusnál gyakori.</span><span class="sxs-lookup"><span data-stu-id="34c79-113">The tag "**WindowsAzureActiveDirectoryIntegratedApp**" is common to all types of apps.</span></span> <span data-ttu-id="34c79-114">Az alábbi kódrészletet használva felsorolhatja az összes SAML-appot (a galériát és a nem galériát is):</span><span class="sxs-lookup"><span data-stu-id="34c79-114">You can use following snippet to list all the SAML apps (both gallery and non-gallery):</span></span>

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    <span data-ttu-id="34c79-115">További információ: [AZ SAML-kompatibilis alkalmazások azonosítása az Azure AD-ban.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)</span><span class="sxs-lookup"><span data-stu-id="34c79-115">For more information, see [Identify SAML-enabled apps in Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span></span>

4. <span data-ttu-id="34c79-116">**Csak a webalkalmazások** kereséséhez és listához: Az alábbi paranccsal szerezze be az összes Azure AD-alkalmazást a "Web app/API" alkalmazástípussal.</span><span class="sxs-lookup"><span data-stu-id="34c79-116">**Find and list only Web applications**: Use the below command to get all Azure AD applications with the application type "Web app/API"</span></span>

    <span data-ttu-id="34c79-117">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT</span><span class="sxs-lookup"><span data-stu-id="34c79-117">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -ne $true } | FT</span></span>
5. <span data-ttu-id="34c79-118">**Csak a natív alkalmazások megkereséséről** és listáról: Futtassa az alábbi parancsot az összes natív ügyfélalkalmazás (asztali/mobileszköz) alkalmazás be szerezze be.</span><span class="sxs-lookup"><span data-stu-id="34c79-118">**Find and list Native applications alone**: Run the following command to get all the native client (desktop/mobile device) applications.</span></span>

    <span data-ttu-id="34c79-119">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT</span><span class="sxs-lookup"><span data-stu-id="34c79-119">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -eq $true } | FT</span></span>
6. <span data-ttu-id="34c79-120">**Az összes regisztrált Azure AD-alkalmazás részleteinek** exportálása CSV-fájlba: Az alábbi parancs exportálja az összes Azure AD-appot a szükséges adatokkal a CSV-fájlba:</span><span class="sxs-lookup"><span data-stu-id="34c79-120">**Export All Registered Azure AD Application Details to CSV**: The below command exports all the Azure AD apps with required details to csv file:</span></span>

    - <span data-ttu-id="34c79-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span><span class="sxs-lookup"><span data-stu-id="34c79-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span></span>
    - <span data-ttu-id="34c79-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span><span class="sxs-lookup"><span data-stu-id="34c79-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span></span>

7. <span data-ttu-id="34c79-123">**Exportálni kell a nem használt Azure-appok listáját** – Naplójelentés</span><span class="sxs-lookup"><span data-stu-id="34c79-123">**Need to export a list of unused Azure apps** – Audit report</span></span>

    <span data-ttu-id="34c79-124">Az Azure AD legfeljebb 30 napig képes az alkalmazásnaplók megtekintésére, feltéve hogy rendelkezik Azure AD Premium-licenccel.</span><span class="sxs-lookup"><span data-stu-id="34c79-124">Azure AD can show application logs for only up to 30 days provided you have Azure AD Premium license.</span></span>
    <span data-ttu-id="34c79-125">Két lehetőség közül választhat, hogy 30 napnál tovább megőrizze az adatokat.</span><span class="sxs-lookup"><span data-stu-id="34c79-125">You have two options to retain the data for longer than 30 days.</span></span> <span data-ttu-id="34c79-126">Az Azure [AD reporting API-k](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) használatával programozással beolvashatja és adatbázisba tárolhatja az adatokat.</span><span class="sxs-lookup"><span data-stu-id="34c79-126">You can use the [Azure AD Reporting APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) to retrieve the data programmatically and store it in a database.</span></span> <span data-ttu-id="34c79-127">Másik lehetőségként integrálhatja az auditnaplókat egy külső SIEM-rendszerbe.</span><span class="sxs-lookup"><span data-stu-id="34c79-127">Alternatively, you can integrate audit logs into a third party SIEM system.</span></span>

    <span data-ttu-id="34c79-128">Az összes alkalmazás és tulajdonú alkalmazás applistát letöltheti az Azure Active Directory>alkalmazás-regisztrációk>Az összes alkalmazás/tulajdonú alkalmazás letöltése>alatt.</span><span class="sxs-lookup"><span data-stu-id="34c79-128">You can also download the app list for all applications and owned applications under Azure Active directory>App Registrations>Download>All applications/Owned applications.</span></span>

    <span data-ttu-id="34c79-129">Az alkalmazáslistát az MS Graph szolgáltatáson keresztül a [Listaalkalmazások – Microsoft Graph 1.0-s](https://docs.microsoft.com/graph/api/application-list) és alkalmazáserőforrás-típus – Microsoft Graph [1.0-s](https://docs.microsoft.com/graph/api/resources/application)verziójában talál.</span><span class="sxs-lookup"><span data-stu-id="34c79-129">To get a list of applications through MS Graph, see [List applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) and [application resource type - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span></span>
