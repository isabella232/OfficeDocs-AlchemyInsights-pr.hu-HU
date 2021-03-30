---
title: Azure Active Directory-csatlakozás
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
- "9003257"
- "9890"
ms.openlocfilehash: 59e3798131956847a61af2416c2e4210199cffa5
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405058"
---
# <a name="azure-active-directory-join"></a>Azure Active Directory-csatlakozás

1. Ha első alkalommal hoz létre eszközregisztrációkat, ellenőrizze, hogy áttekinti-e a Bevezetés az eszközkezelésbe az [Azure Active Directoryban](/azure/active-directory/devices/overview) – útmutatót arról, hogy miként irányíthatja az eszközöket az Azure AD-be. 
1. Ha közvetlenül regisztrál eszközöket az Azure AD-be, és regisztrálja őket az Intune-ba, [](/mem/intune/fundamentals/licenses-assign) először meg kell bizonyosodnia arról, hogy konfigurálta az [Intune-t,](/mem/intune/enrollment/device-enrollment) és megfelelően beállította a licencelést.
1. Győződjön meg arról, hogy jogosult műveletek elvégzésére az Azure AD-ban. Az eszközregisztrációk beállításait csak az Azure AD-beli globális rendszergazdák kezelhetik.
1. Az Azure AD-csatlakozás implementációról Az [Azure AD Join](/azure/active-directory/devices/azureadjoin-plan)megtervz.

Az Azure AD-csatlakozással kapcsolatos gyakori problémák megoldásáról további információt a Gyakori kérdések az [Azure AD-hez](/azure/active-directory/devices/faq) való csatlakozásról és a Windows 10 Pro rendszerű eszközökről a Nem lehet [csatlakozni a Windows 10 Pro](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)rendszerű számítógéphez az Azure AD-be – Frissíteni kell a következőre: - Microsoft Community című témakörben olvashat.
