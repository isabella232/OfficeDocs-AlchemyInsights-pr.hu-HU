---
title: Letiltott a feltételes hozzáférés tartományhoz kötött eszközzel
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/20/2021
ms.locfileid: "51036699"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a>Letiltott a feltételes hozzáférés tartományhoz kötött eszközzel

**Erősen ajánlott eszközök**

[Eszközregisztrációs hibaelhárító eszköz](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – Ez az eszköz segít elhárítani a leggyakoribb eszközregisztrációs problémákat.

[Eszközregisztrációs kapcsolat tesztelése parancsprogram](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – Ez a parancsfájl segít biztosítani, hogy egy eszköz hozzáférjen a rendszerfiók eszközregisztrációs végpontjaihoz.

[Azure AD device cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) – Ez a parancsfájl lehetővé teszi a elavult eszközök keresését és kezelését a környezetében.

Íme néhány gyakori ok, amiért előfordulhat, hogy a feltételes hozzáférés nem sikerül egy tartományhoz csatlakozott eszköz (hibrid Azure AD).

1. **Nincs Azure AD PRT** az eszközön – Meg kell győződni arról, hogy az eszközön Azure AD primary Refresh Token (PRT) van. A PRT-ről további információt ebben a dokumentumban [található.](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)

Az Azure AD PRT ellenőrzéséhez futtassa az eszközön a parancsot, és ellenőrizze, hogy az `dsregcmd/status` "AzureAdPrt" egyenlő-e az "IGEN" értékkel.

Ha az "AzureAdPrt" a "NEM" szó, ellenőrizze az alábbiakat:

- Függetlenül attól, hogy összevont környezete van-e az **AD FS használatával,** és ez a környezet nem érhető el a felhasználók otthoni hálózataiból: Ebben az esetben gondoskodjon arról, hogy a "felhasználónévvel átietett" végpontok elérhetők legyenek az extranetből. Ha az AD FS VPN mögött van, győződjön meg arról, hogy a felhasználók csatlakoznak a VPN-hez, és újra bejelentkeznek az eszközre. További információ ebben a [dokumentumban található.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains)

- **Hogy az eszköz TPM-eszköze** hibás-e, és így nem tudja hitelesíteni az eszközt: Ellenőrizze a "tpm.msc" ellenőrzőt, és ellenőrizze, hogy a TPM állapota "Ready" (Készen áll-e). Ha nem, futtassa, és hagyja, hogy az eszköz újra `dsregcmd/leave` csatlakozzon az Azure AD-hez. Ezután próbálkozzon újra. További információ ebben a [dokumentumban található.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)

- **Külső identitásszolgáltatót használ,** amely nem támogatja a WS-Trust protokollt. A dokumentumokban leírtak szerint a hibrid Azure AD-hez csatlakozású eszközök ebben az esetben nem működnek. Kérjük, forduljon az identitásszolgáltatójához segítségért.

2. A felhasználók a Chrome böngészőt **Windows 10-fiókok** vagy Office-bővítmény nélkül használják: A Chrome nem használja automatikusan a **PRT-t az AAD-hez vagy hibrid-AAD-hez** csatlakozású eszközökön: Ez bármilyen eszközalapú feltételes hozzáférési házirend sikertelenségéhez vezet, és a "Nem regisztrált eszköz" hibaüzenet jelenik meg. A Chrome-böngésző megfelelő használatához az SCCM-en vagy az Intune-on keresztül telepítenie kell a "Windows 10-fiókok" vagy "Office-bővítmények a felhasználók Chrome böngészőjéhez" szoftvert. További információ ebben a [dokumentumban található.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)

Ha a bővítményt nem lehet távoli leküldéses módban leküldéses módban elvégezni, értesítse a felhasználókat, hogy a fenti bővítmények közül manuálisan telepítsék az alkalmazásokat az eszközalapú feltételes hozzáférés mögötti hozzáférés érdekében. További információ ebben a [dokumentumban található.](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites)

3. Az eszköz megfelelően hibrid Azure AD-hez csatlakozott, de véletlenül törlődött vagy le lett tiltva, akár az **Azure AD Connectben,** akár az Azure Portalon történt szinkronizálási változások miatt: Ebben az esetben az eszközobjektum a továbbiakban nem ismerhető fel teljesen összekapcsolt eszközként annak ellenére, hogy az "AzureAdJoined" és a "PRT" állapot érvényesként jelenik meg az eszközön.

A probléma megoldásához futtassa az érintett eszközökön, és hagyja, hogy újracsatlakoztassanak az `dsregcmd/leave` Azure AD-hez. További információ ebben a [dokumentumban található.](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices)

> [!NOTE]
> Ha eszközei Windows 10 1809-es frissítéssel, VPN/felhőproxyval vannak frissítve, és problémákat látnak az "AzureAdPrt" állapottal vagy bármilyen SSO-problémával rendelkező appban (az Outlook nem csatlakozik a postaládához a PRT használata nélkül), győződjön meg arról, hogy a [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) vagy az áprilisi kumulatív [frissítés KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) frissítést használva akadályozza meg a PRT-hibákat az ilyen gépeken.

















