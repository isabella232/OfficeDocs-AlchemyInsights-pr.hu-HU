---
title: Single-Sign Azure Active Directoryhoz csatlakozott eszközök esetén
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
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405047"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a><span data-ttu-id="311c7-102">Egyszeri bejelentkezés az Azure Active Directoryhoz csatlakozott eszközökhöz</span><span class="sxs-lookup"><span data-stu-id="311c7-102">Single-sign on for Azure Active Directory Joined Devices</span></span>

<span data-ttu-id="311c7-103">Ha helyszíni Active Directory -környezetben (AD-ben) szeretne csatlakozni az AD-hez tartományhoz illesztett számítógépéhez az Azure AD-hez, ezt a hibrid Azure AD-csatlakozást elvégezve használhatja.</span><span class="sxs-lookup"><span data-stu-id="311c7-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="311c7-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span><span class="sxs-lookup"><span data-stu-id="311c7-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

[<span data-ttu-id="311c7-105">Az Azure AD-hez csatlakozott eszközök konfigurálása helyszíni Single-Sign a Vállalati Windows Hello használatával</span><span class="sxs-lookup"><span data-stu-id="311c7-105">Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business</span></span>](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

<span data-ttu-id="311c7-106">**Az elsődleges frissítési jogkivonattal (PRT) kapcsolatos problémák** Az elsődleges frissítési jogkivonat (PRT) az Azure AD-hitelesítés kulcsfontosságú eleme Windows 10,Windows Server 2016 és újabb verziók, iOS és Android rendszerű eszközökön.</span><span class="sxs-lookup"><span data-stu-id="311c7-106">**Primary Refresh Token (PRT) issues** A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="311c7-107">Ez egy JSON Web Token (JWT), amelyet kifejezetten a Microsoft első fél jogkivonat-közvetítőinek adtak ki, hogy engedélyezzék az egyszeri bejelentkezést az eszközökön használt alkalmazásokban.</span><span class="sxs-lookup"><span data-stu-id="311c7-107">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="311c7-108">A Mi az elsődleges frissítési [jogkivonat?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)2010- és 2013-as verzióban részletes információkat nyújtunk a PRT-tanúsítványok Windows 10-es eszközökön való kibocsátásának, használatával és védelmével kapcsolatosakról.</span><span class="sxs-lookup"><span data-stu-id="311c7-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.</span></span>

<span data-ttu-id="311c7-109">**WamDefaultSet: YES és AzureADPrt: YES** Ezek a mezők azt jelzik, hogy a felhasználó sikeresen hitelesítve lett-e az Azure AD számára az eszközre való adatokat bejelentkezve.</span><span class="sxs-lookup"><span data-stu-id="311c7-109">**WamDefaultSet: YES and AzureADPrt: YES** These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="311c7-110">Ha az értékek **NEM,** annak az oka a következő lehet:</span><span class="sxs-lookup"><span data-stu-id="311c7-110">If the values are **NO**, it could be due:</span></span>

- <span data-ttu-id="311c7-111">A regisztrációkor az eszközhöz társított TPM-hez tartozó hibás tárkulcs (rendszergazdai jogú futtatás esetén ellenőrizze a KeySignTestet).</span><span class="sxs-lookup"><span data-stu-id="311c7-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span></span>
- <span data-ttu-id="311c7-112">Másodlagos bejelentkezési azonosító</span><span class="sxs-lookup"><span data-stu-id="311c7-112">Alternate Login ID</span></span>
- <span data-ttu-id="311c7-113">A HTTP-proxy nem található</span><span class="sxs-lookup"><span data-stu-id="311c7-113">HTTP Proxy not found</span></span>

<span data-ttu-id="311c7-114">Eszközök hibaelhárítása a dsregcmd paranccsal – [SSO állapot](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="311c7-114">Troubleshoot devices using the dsregcmd command - [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span></span>
