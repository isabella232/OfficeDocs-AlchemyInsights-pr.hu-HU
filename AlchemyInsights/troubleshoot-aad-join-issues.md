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
ms.openlocfilehash: 0e9f7c95cf522340e9976f668c1d1a9eaff71910
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405127"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Az Azure AD-beli csatlakozással kapcsolatos hibák elhárítása

1. Ha első alkalommal hoz létre eszközregisztrációkat, ellenőrizze, hogy áttekinti-e a Bevezetés az eszközkezelésbe az [Azure Active Directoryban](https://docs.microsoft.com/azure/active-directory/devices/overview) – útmutatót arról, hogy miként irányíthatja az eszközöket az Azure AD-be. 
1. Ha közvetlenül regisztrál eszközöket az Azure AD-be, és regisztrálja őket az Intune-ba, [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) először meg kell bizonyosodnia arról, hogy konfigurálta az [Intune-t,](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) és megfelelően beállította a licencelést.
1. Győződjön meg arról, hogy jogosult műveletek elvégzésére az Azure AD-ban. Az eszközregisztrációk beállításait csak az Azure AD-beli globális rendszergazdák kezelhetik.
1. Az Azure AD-csatlakozás implementációról Az [Azure AD Join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan)megtervz.

Az Azure AD-hez való csatlakozással kapcsolatos gyakori problémák megoldásáról további információt a Gyakori kérdések az [Azure AD-hez](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) való csatlakozásról és a Windows 10 Pro rendszerű eszközökről a Nem lehet [csatlakozni a Windows 10 Pro](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900) rendszerű számítógéphez az Azure AD szolgáltatáshoz – Frissíteni kell a következőre: - Microsoft Community című témakört.
