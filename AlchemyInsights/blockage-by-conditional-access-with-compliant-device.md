---
title: Letiltott a feltételes hozzáférés a megfelelő eszközzel
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 240bd25f4d62505202c8cd7ceabe4c1cd3d5c0b5
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035995"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Letiltott a feltételes hozzáférés a megfelelő eszközzel

**Erősen ajánlott eszközök**

- [Eszközregisztrációs hibaelhárító eszköz](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – Egy átfogó eszköz, amely segít elhárítani a leggyakoribb eszközregisztrációs problémákat.
- [Eszközregisztrációs kapcsolat tesztelése parancsprogram](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – Egy olyan eszköz, amely biztosítja, hogy egy eszköz hozzáférjen a rendszerfiók eszközregisztrációs végpontjaihoz.
- [Azure AD-eszköz-tisztítási parancsfájl](https://github.com/mzmaili/AzureADDeviceCleanup) – A elavult eszközök keresésére és kezelésére használható eszköz a környezetében.

Íme néhány gyakori ok, amely miatt előfordulhat, hogy a feltételes  hozzáférés nem felel meg egy megfelelő eszköznek, vagy hogy a felhasználók miért kaphatják meg ezt az üzenetet a szervezeti erőforráshoz való bejelentkezésre vonatkozó kérés során.

1. **Az eszköz nincs kötelező eszközállapotban MDM-sel:**

Ellenőrizze, hogy az eszköz regisztrálva van-e egy jóváhagyott MDM-szolgáltatóval, például az Intune-nal, és kompatibilisként *van-e megjelölve.* Az Intune-nal kapcsolatos további információkért lásd ezt a [dokumentumot.](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) Az eszközök megfelelőségét és az Intune-t az Intune-nal felügyelt eszközök szabályainak beállítása megfelelőségi szabályzat [használatával ismertetése tartalmaz.](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started) Ha problémákat jelentkezik egy eszköz Intune-nal való regisztrálása során, a hibaelhárítással kapcsolatos részletekért keresse meg az Eszközregisztrációs hibák elhárítása a [Microsoftban témakört.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) Az Intune további támogatásához hozzon létre egy támogatási kérelmet. Keresse fel az Intune Súgó és támogatás [lapját.](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport)

2. **Az eszköz nincs a szervezeti hálózathoz csatlakozva:**

A szervezeti erőforrásokhoz való hozzáféréshez az eszköznek közvetlen kapcsolaton vagy virtuális magánhálózaton (VPN) keresztül, valamint a helyi vagy az Azure Active Directory szolgáltatáshoz kell csatlakozva lennie. Ha egy munkahelyi eszközhöz szeretne csatlakozni a szervezeti hálózathoz, tekintse át a Csatlakozás munkahelyi eszközhöz a szervezet [hálózatához.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network) Személyes/BYOD-eszköz regisztrálása: A személyes eszköz regisztrálása a szervezet [hálózatán.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network)

- Ha ellenőrizni tudja, hogy az eszköz csatlakozott-e [](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) a hálózathoz, kövesse a regisztrált eszközök vagy a munkahelyi eszközök itt található [lépéseit.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined) A szervezeti hálózati kapcsolatokra vonatkozó kérdésre az alábbi útmutatásokat kell követnie:

    1. Jelentkezzen be a Windowsba a munkahelyi vagy iskolai fiókjával, például a alain@contoso.com.
    2. Csatlakozzon szervezete hálózatához VPN- vagy DirectAccess-kapcsolaton keresztül.
    3. Miután csatlakozott, a **Windows billentyű+L** billentyűkombinációt lenyomva zárolja az eszközt.
    4. Oldja fel az eszköz zárolását a munkahelyi vagy iskolai fiókjával, majd próbálja meg újból elérni a problémás alkalmazást vagy szolgáltatást.

Ha ismét megjelenik a Nem jut el **innen** hibaüzenet, a probléma valószínűleg máshol is megjelenik.

3. **Az operációs rendszer nem támogatott:**

Győződjön meg arról, hogy az operációs rendszer támogatott verzióját futtatja, beleértve az alábbiakat:

- **Windows Client:** Windows 7 vagy újabb

- **Windows Server:** Windows Server 2008 R2 vagy újabb

- **macOS**: macOS X vagy újabb

- **Android és iOS:** Az Android és iOS mobil operációs rendszereinek legújabb verziója

4. **A webböngésző nem támogatott:**

Keresse meg alább a támogatott böngészőket. A Chrome Windows 1703-as vagy újabb verzióival való támogatásához Windows 10-fiókok kiterjesztésre van szükség. Az Edge 85+ esetén a felhasználónak be kell jelentkezve lennie ahhoz, hogy megfelelően adja át az eszközök megfelelőségi adatait. További részleteket itt [talál.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)

- **Windows 10:** Microsoft Edge, Internet Explorer, Chrome
- **Windows 8/8.1**: Internet Explorer, Chrome
- **Windows 7 esetén:** Internet Explorer, Chrome
- **iOS:** Microsoft Edge, Intune Felügyelt böngésző, Safari
- **Android:** **Microsoft Edge:** Intune Felügyelt böngésző, Chrome
- **Windows Phone:** Microsoft Edge, Internet Explorer
- **Windows Server 2019:** Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016:** Internet Explorer
- **Windows Server 2012 R2:** Internet Explorer
- **Windows Server 2008 R2:** Internet Explorer
- **macOS**: Chrome, Safari

További információt a Nem jut el az üzenethez **és** a hibaelhárítási lépésekről itt [talál.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation)
