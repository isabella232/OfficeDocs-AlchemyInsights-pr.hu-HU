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
ms.openlocfilehash: 872333e13bb51b3a22431154627ad561f6db88c681c9eeee523fdd09e58c0371
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039248"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Az Azure AD-hez csatlakozott eszközök egyszeri bejelentkezéssel kapcsolatos problémáinak elhárítása

Ha helyszíni Active Directory -környezetben (AD-ben) szeretne csatlakozni az AD-hez tartományhoz illesztett számítógépéhez az Azure AD-hez, ezt a hibrid Azure AD-csatlakozást elvégezve használhatja. [How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.

További információért lásd: Az Azure AD-hez csatlakozott eszközök konfigurálása helyszíni Single-Sign A Windows Hello [vállalati verzió használata esetén.](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)

**Az elsődleges frissítési jogkivonattal (PRT) kapcsolatos problémák**

Az elsődleges frissítési jogkivonat (PRT) az Azure AD-hitelesítés kulcsfontosságú Windows 10, Windows Server 2016, illetve újabb verzióiban, iOS- és Android-eszközökön. Ez egy JSON Web Token (JWT), amelyet kifejezetten a Microsoft első fél jogkivonat-közvetítőinek adtak ki, hogy engedélyezzék az egyszeri bejelentkezést az eszközökön használt alkalmazásokban. A PRT-tanúsítványok kibocsátásának, használatával és Windows 10 védelmével kapcsolatos részletekért lásd: Mi az elsődleges frissítési [jogkivonat?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: YES és AzureADPrt: YES**

Ezek a mezők azt jelzik, hogy a felhasználó sikeresen hitelesítve lett-e az Azure AD számára az eszközre való adatokat bejelentkezve. Ha az értékek **NEM,** annak oka a következő lehet:

- Hibás tárkulcs az eszközhöz regisztrációkor társított TPM-modulban (ellenőrizze a KeySignTestet emelt szintű futtatáskor)
- Másodlagos bejelentkezési azonosító
- A HTTP-proxy nem található

A dsregcmd paranccsal kapcsolatos hibák elhárításához lásd: [SSO state (SSO állapot).](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
