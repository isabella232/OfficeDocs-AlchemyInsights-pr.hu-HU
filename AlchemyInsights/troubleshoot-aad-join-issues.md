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
# <a name="troubleshoot-azure-ad-join-issues"></a><span data-ttu-id="0bc76-102">Az Azure AD-beli csatlakozással kapcsolatos hibák elhárítása</span><span class="sxs-lookup"><span data-stu-id="0bc76-102">Troubleshoot Azure AD join issues</span></span>

1. <span data-ttu-id="0bc76-103">Ha első alkalommal hoz létre eszközregisztrációkat, ellenőrizze, hogy áttekinti-e a Bevezetés az eszközkezelésbe az [Azure Active Directoryban](https://docs.microsoft.com/azure/active-directory/devices/overview) – útmutatót arról, hogy miként irányíthatja az eszközöket az Azure AD-be.</span><span class="sxs-lookup"><span data-stu-id="0bc76-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="0bc76-104">Ha közvetlenül regisztrál eszközöket az Azure AD-be, és regisztrálja őket az Intune-ba, [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) először meg kell bizonyosodnia arról, hogy konfigurálta az [Intune-t,](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) és megfelelően beállította a licencelést.</span><span class="sxs-lookup"><span data-stu-id="0bc76-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="0bc76-105">Győződjön meg arról, hogy jogosult műveletek elvégzésére az Azure AD-ban.</span><span class="sxs-lookup"><span data-stu-id="0bc76-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="0bc76-106">Az eszközregisztrációk beállításait csak az Azure AD-beli globális rendszergazdák kezelhetik.</span><span class="sxs-lookup"><span data-stu-id="0bc76-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="0bc76-107">Az Azure AD-csatlakozás implementációról Az [Azure AD Join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan)megtervz.</span><span class="sxs-lookup"><span data-stu-id="0bc76-107">To do Azure AD join implementation, see [Plan Azure AD Join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="0bc76-108">Az Azure AD-hez való csatlakozással kapcsolatos gyakori problémák megoldásáról további információt a Gyakori kérdések az [Azure AD-hez](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) való csatlakozásról és a Windows 10 Pro rendszerű eszközökről a Nem lehet [csatlakozni a Windows 10 Pro](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900) rendszerű számítógéphez az Azure AD szolgáltatáshoz – Frissíteni kell a következőre: - Microsoft Community című témakört.</span><span class="sxs-lookup"><span data-stu-id="0bc76-108">For more details on resolving  common issues with Azure AD join see [Azure Ad Join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)</span></span>
