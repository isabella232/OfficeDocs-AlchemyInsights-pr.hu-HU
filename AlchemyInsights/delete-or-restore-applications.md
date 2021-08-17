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
ms.openlocfilehash: 0c7be98650ca87f36b66f0bb38fb665fc81525b7f3410da14b99fb67468c1e73
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102573"
---
# <a name="delete-or-restore-applications"></a>Alkalmazások törlése vagy visszaállítása

**Alkalmazás törlése az Azure AD-bérlőből:**

1. Az **Azure AD portálon válassza** a **Nagyvállalati alkalmazások lehetőséget.** Ezután keresse meg és jelölje ki a törölni kívánt alkalmazást.
2. A bal **oldali ablaktábla** Kezelés szakaszában válassza a Tulajdonságok **lehetőséget.**
3. Válassza **a Törlés** gombot, majd az **Igen** gombot az alkalmazás Azure AD-bérlőből való törlésének megerősítéséhez.

Az appok törléséről további információt a Gyorsútmutató: Alkalmazás törlése az Azure Active Directory [(Azure AD) bérlői webhelyről.](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)

A PowerShellben a [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) parancsmag eltávolítja az alkalmazás proxykonfigurációit az Azure Active Directory-ban egy adott alkalmazásból, és teljes egészében törölheti az alkalmazást, ha meg van adva.

A törölt **alkalmazásokat visszaállíthatja a** PowerShell használatával. Miután azonosította a visszaállítani kívánt alkalmazást, a [Restore-AzureADDeletedApplication használatával visszaállíthatja.](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
