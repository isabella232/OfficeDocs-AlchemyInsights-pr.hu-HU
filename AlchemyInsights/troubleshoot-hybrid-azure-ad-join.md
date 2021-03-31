---
title: Hybrid Azure AD csatlakozás
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401909"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a><span data-ttu-id="7d170-102">Hybrid Azure AD csatlakozás</span><span class="sxs-lookup"><span data-stu-id="7d170-102">Troubleshoot Hybrid Azure AD join</span></span>

<span data-ttu-id="7d170-103">Erősen ajánlott annak biztosítása, hogy egy eszköz hozzáférjen a rendszerfiókban található eszköz-regisztráció végpontjaihoz az [eszköz-regisztráció csatlakozási parancsprogramjának](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) használatával.</span><span class="sxs-lookup"><span data-stu-id="7d170-103">Highly Recommended Ensure that a device can access Device Registration endpoints under the system account by using the [Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span></span>

1. <span data-ttu-id="7d170-104">Ha első alkalommal hoz létre eszközregisztrációkat, tekintse át a [Bevezetés az Azure Active Directory eszközkezelésbe](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) témakört, és megtudhatja, hogy miként irányíthatja az eszközöket az Azure AD ellenőrzése alatt.</span><span class="sxs-lookup"><span data-stu-id="7d170-104">If you are setting up device registrations for the first time, be sure to review I[ntroduction to device management in Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) to learn how to get devices under the control of Azure AD.</span></span>
1. <span data-ttu-id="7d170-105">Ha közvetlenül regisztrál eszközöket az Azure AD-be, és feliratkozik velük az Intune-ba, akkor győződjön meg arról, hogy [konfigurálta az Intune-t](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support), és elsőként a [licencelést](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) jelölte meg.</span><span class="sxs-lookup"><span data-stu-id="7d170-105">If you are registering devices into Azure AD directly and enrolling them into Intune, be sure that you've [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
1. <span data-ttu-id="7d170-106">Győződjön meg arról, hogy jogosult műveletek elvégzésére az Azure AD-ban és a helyszíni AD-ban.</span><span class="sxs-lookup"><span data-stu-id="7d170-106">Ensure that you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="7d170-107">Az eszközregisztrációk beállításait csak az Azure AD globális rendszergazdája kezelheti.</span><span class="sxs-lookup"><span data-stu-id="7d170-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="7d170-108">Ezenkívül ha automatikus regisztrációt hoz létre a helyszíni Active Directoryban, akkor az Active Directory és az Active Directory FS (ha van) rendszergazdájának kell lennie.</span><span class="sxs-lookup"><span data-stu-id="7d170-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="7d170-109">A hibrid illesztés esetleges problémáinak megoldásáról lásd [A hibrid csatlakozás hibaelhárítása](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) témakört a hibrid Azure AD-eszközökhöz való csatlakozásról, valamint az eszközkezelés az Azure AD portálon keresztüli beállításáról lásd [Az Azure AD-hez csatlakozott hibrid eszközök beállítása](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) és az [Eszközök kezelése az Azure portal használatával](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support) témaköröket.</span><span class="sxs-lookup"><span data-stu-id="7d170-109">For more details on resolve potential issues with Hybrid join, see [Troubleshoot Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) for set up hybrid Azure AD joined and Manage Devices using Azure Ad portal, see [Set up hybrid Azure AD joined (on-premises domain-joined) devices](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) and [Manage devices using the Azure portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="7d170-110">A hibrid Azure Active Directory csatlakozás gyakori problémáinak megoldásáról lásd: [Az Azure AD-hez való hibrid csatlakozás - gyakori kérdések](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span><span class="sxs-lookup"><span data-stu-id="7d170-110">To resolve common issues with Hybrid Azure Active Directory (AD) join, see [Hybrid Azure AD join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span></span>
