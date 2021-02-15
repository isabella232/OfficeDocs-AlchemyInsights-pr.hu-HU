---
title: A jelszóvisszaírás nem működik
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243367"
---
# <a name="password-writeback-is-not-working"></a>A jelszóvisszaírás nem működik

**Problémákat tapasztalok a jelszó-visszaírás konfigurálásával kapcsolatban**

- A jelszóvisszaírás egy prémium funkció.
- Győződjön meg arról, hogy megértette a licencelési követelményeket:
  - A szervezetéhez legalább egy licencnek hozzá kell rendelnie
  - **Csak felhőbeli felhasználók** – Bármely Office 365 -ös (O365) fizetős termékváltozat vagy Azure AD Basic
  - **Felhőbeli és/vagy helyszíni** felhasználók – Azure AD Premium P1 vagy P2, Enterprise Mobility + Security (EMS) vagy Secure Productive Enterprise (SPE)
    - A licencelési követelményekről az [Azure AD önkiszolgáló jelszó-visszaállítási](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing) licencelési követelményeiben olvashat bővebben.
- Legalább egy rendszergazdai fiókkal és egy tesztfelhasználói fiókkal rendelkezik a megfelelő licenccel.
- A jelszó-visszaíráshoz csatlakoztatnia kell az Azure AD Connectet az elsődleges tartományvezérlő emulátorához. Beállíthatja úgy az Azure AD Connectet, hogy  elsődleges tartományvezérlőt használjon. Kattintson a jobb gombbal az Active Directory szinkronizálási összekötő tulajdonságaira, és válassza a címtárpartíciók **konfigurálása parancsot.** Itt keresse meg a **tartományvezérlő** kapcsolati beállításainak szakaszát, és jelölje be a jelölőnégyzetet, amely csak előnyben részesített **tartományvezérlőket használ.**
  > [!NOTE]
  > Ha az előnyben részesített tartományvezérlő nem PDC-emulátor, az Azure AD Connect továbbra is kapcsolatba fog lépjen a pdc-nek jelszó-visszaírásért.
- A bérlői fiókban beállította és engedélyezte a jelszó-visszaállítást. További információt az Azure AD-jelszavak alaphelyzetbe állításának [engedélyezése a felhasználók számára.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- Győződjön meg arról, hogy a jelszó-visszaírás engedélyezéséhez használt rendszergazdai fiók egy felhőbeli rendszergazdai fiók (amely nem helyszíni AD-ban jött létre az Azure AD-ban)
- A Windows Server 2008 R2, a Windows Server 2012 vagy a Windows Server 2012 R2 rendszert futtató helyszíni AD-telepítésben telepítve van a legújabb szervizcsomagok
- Telepítve van az Azure AD Connect eszköz, és előkészítette az AD-környezetet a felhőbe való szinkronizáláshoz. A jelszóvisszaírás tesztelése előtt győződjön meg arról, hogy először teljes körű importálást és teljes szinkronizálást végzett az Azure AD Connectben az AD és az Azure AD szolgáltatásból.
- További információ: teljes szinkronizálás és teljes importálás az [Azure AD Connectben](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Probléma van a jelszó-visszaírási kapcsolattal**

1. Az Azure AD Connect legújabb [verziójának letöltése és engedélyezése](https://www.microsoft.com/download/details.aspx?id=47594)
2. Tűzfalkonfiguráció: Az Azure AD Connect eszköznek (1.1.443-as vagy fenti) kimenő **HTTPS-hozzáférésre** van szüksége a következő szolgáltatásokhoz:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Az üresjárati kapcsolatok megőrzésének engedélyezése legalább 2–3 percig

**Továbbra is problémákat tapasztalok a jelszó-visszaírással kapcsolatban**

- Ha továbbra is nehézségekbe ütközik, próbálja meg letiltani és újra engedélyezni a jelszóvisszaírási szolgáltatást az Azure AD Connect eszközben
- További információ a [jelszóvisszaírás](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot) letiltásához és újra engedélyezéséhez
