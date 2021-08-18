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
ms.openlocfilehash: 679dea6d488cf74f51baee2b3b498dc64b95530e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324925"
---
# <a name="password-writeback-is-not-working"></a>Nem működik a jelszóvisszaírás

**Problémákat tapasztalok a jelszó-visszaírás konfigurálásakor**

- A jelszóvisszaírás egy prémium funkció.
- Győződjön meg arról, hogy megértette a licencelési követelményeket:
  - Legalább egy licencnek hozzá kell rendelnie a szervezetéhez
  - **Csak felhőbeli felhasználók** – Office 365 (O365) fizetős termékváltozat vagy Azure AD Basic
  - **Felhőbeli és/vagy** helyszíni felhasználók – Prémium P1 szintű Azure AD P2, Enterprise Mobility + Security (EMS) vagy Secure Productive Enterprise (SPE)
    - A licencelési követelményekről az [Azure AD önkiszolgáló jelszó-visszaállítási](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing) licenckövetelményei
- Legalább egy rendszergazdai fiókkal és egy tesztfiókkal rendelkezik a megfelelő licenccel.
- Ahhoz, hogy működjön a jelszó-Csatlakozás, csatlakoztatnia kell az Azure AD-Emulator elsődleges tartományvezérlőhöz. Az Azure AD Csatlakozás konfigurálható elsődleges tartományvezérlő használatára: kattintson  a jobb gombbal az Active Directory szinkronizálási összekötő tulajdonságaira, majd válassza a címtárpartíciók **konfigurálása parancsot.** Itt keresse meg a **Tartományvezérlők** kapcsolati beállításai szakaszt, és jelölje be a Csak előnyben részesített tartományvezérlők használata című **jelölőnégyzetet.**
    **Megjegyzés:** Ha az előnyben részesített tartományvezérlő nem PDC-emulátor, az Azure AD Csatlakozás továbbra is el fogja érni a pdc-et jelszó-visszaírásért.
- A jelszó alaphelyzetbe állítása be lett állítva és engedélyezett a bérlői fiókban. További információ: Azure AD-jelszavak alaphelyzetbe állításának [engedélyezése a felhasználóknak.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- Győződjön meg arról, hogy a jelszó-visszaírás engedélyezéséhez használt rendszergazdai fiók egy (nem helyszíni Azure AD-ban létrehozott) felhőbeli rendszergazdai fiók.
- Egyetlen vagy többerdőS AD helyszíni telepítésű, Windows Server 2008 R2, Windows Server 2012 vagy Windows Server 2012 R2 telepített szervizcsomaggal
- Telepítve van az Azure AD Csatlakozás eszköz, és előkészítette az AD-környezetet a felhővel való szinkronizáláshoz. A jelszó-visszaírás tesztelése előtt győződjön meg arról, hogy az Azure AD-beli Azure AD szolgáltatásban az AD-ről és az Azure AD-ről egyaránt teljes körű és teljes szinkronizálást Csatlakozás.
- További információ: Teljes szinkronizálás és teljes importálás az [Azure AD-Csatlakozás](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Probléma a jelszó-visszaírási kapcsolattal**

1. Az Azure AD-szolgáltatások legújabb [verziójának letöltése és Csatlakozás](https://www.microsoft.com/download/details.aspx?id=47594)
2. Tűzfalkonfiguráció: Az Azure AD Csatlakozás eszköznek (1.1.443-as vagy magasabb) kimenő **HTTPS-hozzáférésre** van szüksége a következő szolgáltatásokhoz:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Az inaktív kapcsolatok megőrzésének engedélyezése legalább 2–3 percig

**Továbbra is problémákat tapasztalok a jelszó-visszaírással kapcsolatban**

- Ha továbbra is problémát okoz, próbálja meg letiltani, majd újra engedélyezni a jelszó-visszaírási szolgáltatást az Azure AD Csatlakozás eszközben
- További információért olvassa el a [jelszó-visszaírás](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot) letiltását és újra engedélyezését
