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
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Az Azure AD-hez csatlakozott eszközök egyszeri bejelentkezéssel kapcsolatos problémáinak elhárítása

Ha helyszíni Active Directory -környezetben (AD-ben) szeretne csatlakozni az AD-hez tartományhoz illesztett számítógépéhez az Azure AD-hez, ezt a hibrid Azure AD-csatlakozást elvégezve használhatja. [How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.

További információt Az Azure AD-hez csatlakozott eszközök konfigurálása helyszíni környezethez [Single-Sign a Windows Hello vállalati verzió használatával.](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)

**Az elsődleges frissítési jogkivonattal (PRT) kapcsolatos problémák**

Az elsődleges frissítési jogkivonat (PRT) az Azure AD-hitelesítés kulcsfontosságú eleme Windows 10,Windows Server 2016 és újabb verziók, iOS és Android rendszerű eszközökön. Ez egy JSON Web Token (JWT), amelyet kifejezetten a Microsoft első fél jogkivonat-közvetítőinek adtak ki, hogy engedélyezzék az egyszeri bejelentkezést az eszközökön használt alkalmazásokban. A PRT-tanúsítványok Windows 10-es eszközökön való kibocsátásának, használatával és védelmével kapcsolatos részletekért lásd: Mi az elsődleges frissítési [jogkivonat?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: YES és AzureADPrt: YES**

Ezek a mezők azt jelzik, hogy a felhasználó sikeresen hitelesítve lett-e az Azure AD számára az eszközre való adatokat bejelentkezve. Ha az értékek **NEM,** annak oka a következő lehet:

- Hibás tárkulcs az eszközhöz regisztrációkor társított TPM-modulban (ellenőrizze a KeySignTestet emelt szintű futtatáskor)
- Másodlagos bejelentkezési azonosító
- A HTTP-proxy nem található

A dsregcmd paranccsal kapcsolatos hibák elhárításához lásd: [SSO state (SSO állapot).](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
