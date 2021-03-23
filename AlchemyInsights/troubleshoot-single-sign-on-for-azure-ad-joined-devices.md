---
title: Az Azure AD-hez csatlakozott eszközök egyszeri bejelentkezéssel kapcsolatos problémáinak elhárítása
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
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036171"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a><span data-ttu-id="26a2e-102">Az Azure AD-hez csatlakozott eszközök egyszeri bejelentkezéssel kapcsolatos problémáinak elhárítása</span><span class="sxs-lookup"><span data-stu-id="26a2e-102">Troubleshoot Single-sign on for Azure AD Joined Devices</span></span>

<span data-ttu-id="26a2e-103">Ha helyszíni Active Directory -környezetben (AD-ben) szeretne csatlakozni az AD-hez tartományhoz illesztett számítógépéhez az Azure AD-hez, ezt a hibrid Azure AD-csatlakozást elvégezve használhatja.</span><span class="sxs-lookup"><span data-stu-id="26a2e-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="26a2e-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span><span class="sxs-lookup"><span data-stu-id="26a2e-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

<span data-ttu-id="26a2e-105">További információt Az Azure AD-hez csatlakozott eszközök konfigurálása helyszíni környezethez [Single-Sign a Windows Hello vállalati verzió használatával.](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)</span><span class="sxs-lookup"><span data-stu-id="26a2e-105">For more information, see [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="26a2e-106">**Az elsődleges frissítési jogkivonattal (PRT) kapcsolatos problémák**</span><span class="sxs-lookup"><span data-stu-id="26a2e-106">**Primary Refresh Token (PRT) issues**</span></span>

<span data-ttu-id="26a2e-107">Az elsődleges frissítési jogkivonat (PRT) az Azure AD-hitelesítés kulcsfontosságú eleme Windows 10,Windows Server 2016 és újabb verziók, iOS és Android rendszerű eszközökön.</span><span class="sxs-lookup"><span data-stu-id="26a2e-107">A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="26a2e-108">Ez egy JSON Web Token (JWT), amelyet kifejezetten a Microsoft első fél jogkivonat-közvetítőinek adtak ki, hogy engedélyezzék az egyszeri bejelentkezést az eszközökön használt alkalmazásokban.</span><span class="sxs-lookup"><span data-stu-id="26a2e-108">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="26a2e-109">A PRT-tanúsítványok Windows 10-es eszközökön való kibocsátásának, használatával és védelmével kapcsolatos részletekért lásd: Mi az elsődleges frissítési [jogkivonat?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="26a2e-109">For details on how a PRT is issued, used, and protected on Windows 10 devices, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="26a2e-110">**WamDefaultSet: YES és AzureADPrt: YES**</span><span class="sxs-lookup"><span data-stu-id="26a2e-110">**WamDefaultSet: YES and AzureADPrt: YES**</span></span>

<span data-ttu-id="26a2e-111">Ezek a mezők azt jelzik, hogy a felhasználó sikeresen hitelesítve lett-e az Azure AD számára az eszközre való adatokat bejelentkezve.</span><span class="sxs-lookup"><span data-stu-id="26a2e-111">These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="26a2e-112">Ha az értékek **NEM,** annak oka a következő lehet:</span><span class="sxs-lookup"><span data-stu-id="26a2e-112">If the values are **NO**, it could be due to:</span></span>

- <span data-ttu-id="26a2e-113">Hibás tárkulcs az eszközhöz regisztrációkor társított TPM-modulban (ellenőrizze a KeySignTestet emelt szintű futtatáskor)</span><span class="sxs-lookup"><span data-stu-id="26a2e-113">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)</span></span>
- <span data-ttu-id="26a2e-114">Másodlagos bejelentkezési azonosító</span><span class="sxs-lookup"><span data-stu-id="26a2e-114">Alternate Login ID</span></span>
- <span data-ttu-id="26a2e-115">A HTTP-proxy nem található</span><span class="sxs-lookup"><span data-stu-id="26a2e-115">HTTP Proxy not found</span></span>

<span data-ttu-id="26a2e-116">A dsregcmd paranccsal kapcsolatos hibák elhárításához lásd: [SSO state (SSO állapot).](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="26a2e-116">To troubleshoot devices using the dsregcmd command, see [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>
