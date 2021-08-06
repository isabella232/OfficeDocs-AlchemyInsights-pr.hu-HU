---
title: Nem működik a jelszóvisszaírás
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
ms.openlocfilehash: 23f5e5fe9e00a4bb00f96d2023c81f6413a7d8b808fd46bfc94483944bb898dc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999746"
---
# <a name="password-writeback-is-not-working"></a>Nem működik a jelszóvisszaírás

**Problémákat tapasztalok a jelszó-visszaírás konfigurálásakor**

- A jelszóvisszaírás egy prémium funkció.
- Győződjön meg arról, hogy megértette a licencelési követelményeket:
  - Legalább egy licencnek hozzá kell rendelnie a szervezetéhez
  - **Csak felhőbeli felhasználók** – Office 365 (O365) díjért fizetett termékváltozat vagy Azure AD Basic
  - **Felhőbeli és/vagy** helyszíni felhasználók – Prémium P1 szintű Azure AD P2, Enterprise Mobility + Security (EMS) vagy Secure Productive Enterprise (SPE)
    - A licencelési követelményekről az [Azure AD önkiszolgáló jelszó-visszaállítási](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing) licenckövetelményei
- Legalább egy rendszergazdai fiókkal és egy tesztfiókkal rendelkezik a megfelelő licenccel.
- Ahhoz, hogy működjön a jelszó-Emulator, csatlakoztatnia kell az Azure AD-Csatlakozás az elsődleges tartományvezérlőhöz. Az Azure AD Csatlakozás konfigurálható elsődleges tartományvezérlő használatára. Kattintson  a jobb gombbal az Active Directory szinkronizálási összekötő tulajdonságaira, majd válassza a címtárpartíciók **konfigurálása parancsot.** Itt keresse meg a **Tartományvezérlők** kapcsolati beállításai szakaszt, és jelölje be a Csak előnyben részesített tartományvezérlők használata című **jelölőnégyzetet.**
  > [!NOTE]
  > Ha az előnyben részesített tartományvezérlő nem PDC emulátor, az Azure AD Csatlakozás a rendszer továbbra is el fogja érni a pdc-et jelszó-visszaírásért.
- A jelszó alaphelyzetbe állítása be lett állítva és engedélyezett a bérlői fiókban. További információt Az [Azure AD-jelszavak](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)alaphelyzetbe állításának engedélyezése a felhasználóknak.
- Győződjön meg arról, hogy a jelszó-visszaírás engedélyezéséhez használt rendszergazdai fiók egy (nem helyszíni Azure AD-ban létrehozott) felhőbeli rendszergazdai fiók.
- Egy vagy többerdőS AD helyszíni telepítésű, Windows Server 2008 R2, Windows Server 2012 vagy Windows Server 2012 R2 telepített szervizcsomaggal
- Telepítve van az Azure AD Csatlakozás eszköz, és előkészítette az AD-környezetet a felhővel való szinkronizáláshoz. Mielőtt tesztelné a jelszóvisszaírást, győződjön meg arról, hogy az Azure AD-beli Azure AD szolgáltatásban az AD-ről és az Azure AD-ről egyaránt teljes körű és teljes szinkronizálást Csatlakozás.
- További információ: Teljes szinkronizálás és teljes importálás az [Azure AD-Csatlakozás](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Probléma a jelszó-visszaírási kapcsolattal**

1. Az Azure AD-szolgáltatások legújabb [verziójának letöltése és Csatlakozás](https://www.microsoft.com/download/details.aspx?id=47594)
2. Tűzfalkonfiguráció: Az Azure AD Csatlakozás eszköznek (1.1.443-as vagy fenti) kimenő **HTTPS-hozzáférést** kell használnia a következőhöz:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Az inaktív kapcsolatok megőrzésének engedélyezése legalább 2–3 percig

**Továbbra is problémákat tapasztalok a jelszó-visszaírással kapcsolatban**

- Ha továbbra is problémát okoz, próbálja meg letiltani, majd újra engedélyezni a jelszó-visszaírási szolgáltatást az Azure AD Csatlakozás eszközben
- További információért olvassa el a [jelszó-visszaírás](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot) letiltását és újra engedélyezését
