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
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Egyszeri bejelentkezés az Azure Active Directoryhoz csatlakozott eszközökhöz

Ha helyszíni Active Directory -környezetben (AD-ben) szeretne csatlakozni az AD-hez tartományhoz illesztett számítógépéhez az Azure AD-hez, ezt a hibrid Azure AD-csatlakozást elvégezve használhatja. [How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.

[Az Azure AD-hez csatlakozott eszközök konfigurálása helyszíni Single-Sign a Vállalati Windows Hello használatával](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Az elsődleges frissítési jogkivonattal (PRT) kapcsolatos problémák** Az elsődleges frissítési jogkivonat (PRT) az Azure AD-hitelesítés kulcsfontosságú eleme Windows 10,Windows Server 2016 és újabb verziók, iOS és Android rendszerű eszközökön. Ez egy JSON Web Token (JWT), amelyet kifejezetten a Microsoft első fél jogkivonat-közvetítőinek adtak ki, hogy engedélyezzék az egyszeri bejelentkezést az eszközökön használt alkalmazásokban. A Mi az elsődleges frissítési [jogkivonat?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)2010- és 2013-as verzióban részletes információkat nyújtunk a PRT-tanúsítványok Windows 10-es eszközökön való kibocsátásának, használatával és védelmével kapcsolatosakról.

**WamDefaultSet: YES és AzureADPrt: YES** Ezek a mezők azt jelzik, hogy a felhasználó sikeresen hitelesítve lett-e az Azure AD számára az eszközre való adatokat bejelentkezve. Ha az értékek **NEM,** annak az oka a következő lehet:

- A regisztrációkor az eszközhöz társított TPM-hez tartozó hibás tárkulcs (rendszergazdai jogú futtatás esetén ellenőrizze a KeySignTestet).
- Másodlagos bejelentkezési azonosító
- A HTTP-proxy nem található

Eszközök hibaelhárítása a dsregcmd paranccsal – [SSO állapot](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
