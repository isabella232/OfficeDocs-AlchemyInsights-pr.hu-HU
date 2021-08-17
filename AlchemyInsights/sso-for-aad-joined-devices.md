---
title: Single-Sign az összekapcsolt Azure Active Directory esetén
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
ms.openlocfilehash: 365225926296677feb7853481651a634792fd8bfa9abd9dc9359ffaae50b60eb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050012"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Egyszeres bejelentkezés az Azure Active Directory eszközökön

Ha helyszíni Active Directory -környezetben (AD-ben) szeretne csatlakozni az AD-hez tartományhoz illesztett számítógépéhez az Azure AD-hez, ezt a hibrid Azure AD-csatlakozást elvégezve használhatja. [How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.

[Az Azure AD-hez csatlakozott eszközök konfigurálása helyszíni Single-Sign a Windows Hello Vállalati verzió használatával](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Az elsődleges frissítési jogkivonattal (PRT) kapcsolatos problémák** Az elsődleges frissítési jogkivonat (PRT) az Azure AD-hitelesítés kulcsfontosságú Windows 10, Windows Server 2016, illetve újabb verzióiban, iOS- és Android-eszközökön. Ez egy JSON Web Token (JWT), amelyet kifejezetten a Microsoft első fél jogkivonat-közvetítőinek adtak ki, hogy engedélyezzék az egyszeri bejelentkezést az eszközökön használt alkalmazásokban. [A Mi az elsődleges](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)frissítési jogkivonat? alatt részletesen meg fogjuk adni a PRT-tanúsítványok kibocsátásának, Windows 10 védelmét.

**WamDefaultSet: YES és AzureADPrt: YES** Ezek a mezők azt jelzik, hogy a felhasználó sikeresen hitelesítve lett-e az Azure AD számára az eszközre való adatokat bejelentkezve. Ha az értékek **NEM,** annak az oka a következő lehet:

- A regisztrációkor az eszközhöz társított TPM-hez tartozó hibás tárkulcs (rendszergazdai jogú futtatás esetén ellenőrizze a KeySignTestet).
- Másodlagos bejelentkezési azonosító
- A HTTP-proxy nem található

Eszközök hibaelhárítása a dsregcmd paranccsal – [SSO állapot](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
