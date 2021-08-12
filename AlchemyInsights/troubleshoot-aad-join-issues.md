---
title: Az Azure AD-beli csatlakozással kapcsolatos hibák elhárítása
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "6157"
ms.openlocfilehash: 8e902aea30e6891717e08027cc009576d390c9cf2ba1649cbbc68d64883937f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939921"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Az Azure AD-beli csatlakozással kapcsolatos hibák elhárítása

1. Ha első alkalommal ad meg eszközregisztrációkat, tekintse át a Bevezetés az eszközkezelésbe az [Azure Active Directory-ban](https://docs.microsoft.com/azure/active-directory/devices/overview) útmutatót arról, hogy miként irányíthatja az eszközöket az Azure AD-be. 
1. Ha közvetlenül regisztrál eszközöket az Azure AD-be, és regisztrálja őket az Intune-ba, [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) először meg kell bizonyosodnia arról, hogy konfigurálta az [Intune-t,](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) és megfelelően beállította a licencelést.
1. Győződjön meg arról, hogy jogosult műveletek elvégzésére az Azure AD-ban. Az eszközregisztrációk beállításait csak az Azure AD globális rendszergazdája kezelheti.
1. Az Azure AD-csatlakozás implementációról Az [Azure AD Join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan)megtervz.

Az Azure AD-hez való csatlakozással kapcsolatos gyakori problémák megoldásáról további információt a Gyakori kérdések az [Azure AD-hez](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) való csatlakozásról és Windows 10 Windows 10 Pro pro eszközről a Nem lehet csatlakozni egy géphez az [Azure AD-be](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900) – Frissíteni kell a következőre: Microsoft Community című témakörben talál.
