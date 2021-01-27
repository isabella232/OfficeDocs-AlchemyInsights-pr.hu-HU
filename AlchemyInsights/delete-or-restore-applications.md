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
# <a name="delete-or-restore-applications"></a>Alkalmazások törlése vagy visszaállítása

**Alkalmazás törlése az Azure AD-bérlőből:**

1. Az **Azure AD portálon válassza** a **Nagyvállalati alkalmazások lehetőséget.** Ezután keresse meg és jelölje ki a törölni kívánt alkalmazást.
2. A bal **oldali ablaktábla** Kezelés szakaszában válassza a **Tulajdonságok lehetőséget.**
3. Válassza **a Törlés** gombot, majd az **Igen** gombot annak megerősítéséhez, hogy törölni szeretné az appot az Azure AD-bérlőből.

Az appok törléséről további információt a Gyorsútmutató: Alkalmazás törlése az [Azure Active Directory (Azure AD) bérlői webhelyről.](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)

A PowerShellben a [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) parancsmag eltávolítja az Alkalmazásproxy-konfigurációkat egy adott alkalmazásból az Azure Active Directoryban, és ha meg van adva, teljes egészében törölheti az alkalmazást.

A PowerShell használatával visszaállíthatja **a** törölt alkalmazásokat. Miután azonosította a visszaállítani kívánt alkalmazást, visszaállíthatja [a Restore-AzureADDeletedApplication használatával.](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
