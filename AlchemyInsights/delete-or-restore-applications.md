---
title: Alkalmazások törlése vagy visszaállítása
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
- "9004335"
- "7737"
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014901"
---
# <a name="delete-or-restore-applications"></a><span data-ttu-id="6db2c-102">Alkalmazások törlése vagy visszaállítása</span><span class="sxs-lookup"><span data-stu-id="6db2c-102">Delete or restore applications</span></span>

<span data-ttu-id="6db2c-103">**Alkalmazás törlése az Azure AD-bérlőből:**</span><span class="sxs-lookup"><span data-stu-id="6db2c-103">**To delete an application from your Azure AD tenant**:</span></span>

1. <span data-ttu-id="6db2c-104">Az **Azure AD portálon válassza** a **Nagyvállalati alkalmazások lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="6db2c-104">In the **Azure AD portal**, select **Enterprise applications**.</span></span> <span data-ttu-id="6db2c-105">Ezután keresse meg és jelölje ki a törölni kívánt alkalmazást.</span><span class="sxs-lookup"><span data-stu-id="6db2c-105">Then find and select the application you want to delete.</span></span>
2. <span data-ttu-id="6db2c-106">A bal **oldali ablaktábla** Kezelés szakaszában válassza a **Tulajdonságok lehetőséget.**</span><span class="sxs-lookup"><span data-stu-id="6db2c-106">In the **Manage** section in the left pane, select **Properties**.</span></span>
3. <span data-ttu-id="6db2c-107">Válassza **a Törlés** gombot, majd az **Igen** gombot annak megerősítéséhez, hogy törölni szeretné az appot az Azure AD-bérlőből.</span><span class="sxs-lookup"><span data-stu-id="6db2c-107">Select **Delete**, and then select **Yes** to confirm you want to delete the app from your Azure AD tenant.</span></span>

<span data-ttu-id="6db2c-108">Az appok törléséről további információt a Gyorsútmutató: Alkalmazás törlése az [Azure Active Directory (Azure AD) bérlői webhelyről.](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)</span><span class="sxs-lookup"><span data-stu-id="6db2c-108">For more information on how to delete an app, see [Quickstart: Delete an application from your Azure Active Directory (Azure AD) tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span></span>

<span data-ttu-id="6db2c-109">A PowerShellben a [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) parancsmag eltávolítja az Alkalmazásproxy-konfigurációkat egy adott alkalmazásból az Azure Active Directoryban, és ha meg van adva, teljes egészében törölheti az alkalmazást.</span><span class="sxs-lookup"><span data-stu-id="6db2c-109">In PowerShell, the [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet removes Application Proxy configurations from a specific application in Azure Active Directory, and can delete the application completely if specified.</span></span>

<span data-ttu-id="6db2c-110">A PowerShell használatával visszaállíthatja **a** törölt alkalmazásokat.</span><span class="sxs-lookup"><span data-stu-id="6db2c-110">You can **restore a deleted application** using PowerShell.</span></span> <span data-ttu-id="6db2c-111">Miután azonosította a visszaállítani kívánt alkalmazást, visszaállíthatja [a Restore-AzureADDeletedApplication használatával.](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)</span><span class="sxs-lookup"><span data-stu-id="6db2c-111">Once the application you want to restore has been identified, you can restore it using [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span></span>
